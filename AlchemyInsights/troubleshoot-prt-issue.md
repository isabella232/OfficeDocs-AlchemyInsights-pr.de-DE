---
title: Problembehandlung bei PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571878"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="5ea26-102">Problembehandlung bei PRT</span><span class="sxs-lookup"><span data-stu-id="5ea26-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="5ea26-103">Damit ein Gerät authentifiziert werden kann, muss es vollständig registriert und in gutem Zustand sein und ein primäres Aktualisierungs Token (PRT) abrufen können.</span><span class="sxs-lookup"><span data-stu-id="5ea26-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="5ea26-104">Für den Prozess der Hybriden Azure AD Beitritts Registrierung müssen sich Geräte in einem Unternehmensnetzwerk befinden.</span><span class="sxs-lookup"><span data-stu-id="5ea26-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="5ea26-105">Es funktioniert auch über VPN, aber es gibt einige Vorbehalte.</span><span class="sxs-lookup"><span data-stu-id="5ea26-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="5ea26-106">Kunden benötigen Unterstützung bei der Problembehandlung bei der Hybrid-Azure AD Anmeldung bei Remote-Arbeitsbedingungen.</span><span class="sxs-lookup"><span data-stu-id="5ea26-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="5ea26-107">Hier ist eine Aufschlüsselung dessen, was passiert "unter der Haube" während des Registrierungsprozesses.</span><span class="sxs-lookup"><span data-stu-id="5ea26-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="5ea26-108">**Cloud-Authentifizierungsumgebung (mit Azure AD Kennworthash Synchronisierung oder Pass-Through-Authentifizierung)**</span><span class="sxs-lookup"><span data-stu-id="5ea26-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="5ea26-109">Dieser Registrierungs Fluss wird auch als "Synchronisierungs Beitritt" bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="5ea26-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="5ea26-110">Windows 10 ermittelt einen SCP-Eintrag, wenn sich der Benutzer am Gerät anmeldet.</span><span class="sxs-lookup"><span data-stu-id="5ea26-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="5ea26-111">Das Gerät versucht zunächst, Mandanteninformationen aus dem clientseitigen SCP in der Registrierung [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] abzurufen.</span><span class="sxs-lookup"><span data-stu-id="5ea26-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="5ea26-112">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="5ea26-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="5ea26-113">Wenn ein Fehler auftritt, kommuniziert das Gerät mit lokalem Active Directory (AD), um Mandanteninformationen aus dem Dienstverbindungspunkt (Service Connection Points, SCP) zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="5ea26-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="5ea26-114">Informationen zum Überprüfen von SCP finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="5ea26-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="5ea26-115">Es wird empfohlen, SCP in der AD zu aktivieren und nur clientseitigen SCP zur erstmaligen Überprüfung zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="5ea26-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="5ea26-116">Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich gegen Azure AD zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="5ea26-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="5ea26-117">Sie können überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann, indem Sie das Verbindungsskript Test Geräteregistrierung verwenden.</span><span class="sxs-lookup"><span data-stu-id="5ea26-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="5ea26-118">Windows 10 generiert ein selbstsigniertes Zertifikat und speichert es unter dem Computerobjekt im lokalen AD.</span><span class="sxs-lookup"><span data-stu-id="5ea26-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="5ea26-119">Dies erfordert eine Sicht auf Domänen Controller.</span><span class="sxs-lookup"><span data-stu-id="5ea26-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="5ea26-120">Ein Device-Objekt, das ein Zertifikat besitzt, wird über Azure AD Connect mit Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="5ea26-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="5ea26-121">Der Synchronisierungszyklus ist standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration Azure AD Connect ab.</span><span class="sxs-lookup"><span data-stu-id="5ea26-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="5ea26-122">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="5ea26-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="5ea26-123">In dieser Phase sollten Sie das Betreff-Gerät im Status "Ausstehend" unter Device Blade of Azure Portal sehen können.</span><span class="sxs-lookup"><span data-stu-id="5ea26-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="5ea26-124">Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="5ea26-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="5ea26-125">Wenn Sie sich auf VPN befinden und ein Logoff-Anmeldevorgang die Domänen Konnektivität beendet, können Sie die Registrierung manuell auslösen:</span><span class="sxs-lookup"><span data-stu-id="5ea26-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="5ea26-126">Stellen Sie eine dsregcmd/Join lokal an der Administratoreingabeaufforderung oder Remote über PSExec auf Ihrem PC aus.</span><span class="sxs-lookup"><span data-stu-id="5ea26-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="5ea26-127">Beispiel: psexec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="5ea26-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="5ea26-128">Weitere Informationen zu Problemen mit dem Hybriden Beitritt finden Sie unter Problem [Behandlung bei Geräten](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="5ea26-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
