---
title: Gerät im Status "Ausstehend"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652188"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="3529e-102">Gerät im Status "Ausstehend"</span><span class="sxs-lookup"><span data-stu-id="3529e-102">Device in pending state</span></span>

<span data-ttu-id="3529e-103">**Voraussetzungen**</span><span class="sxs-lookup"><span data-stu-id="3529e-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="3529e-104">Wenn Sie Geräte Registrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die Einführung in die [Geräteverwaltung in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) überprüft haben, in dem Sie erfahren, wie Sie Geräte unter Kontrolle von Azure AD erhalten.</span><span class="sxs-lookup"><span data-stu-id="3529e-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="3529e-105">Wenn Sie Geräte direkt in Azure AD registrieren und diese in InTune einschreiben, müssen Sie sicherstellen, dass Sie [InTune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) haben und die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) zuerst eingerichtet haben.</span><span class="sxs-lookup"><span data-stu-id="3529e-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="3529e-106">Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD und lokalen AD auszuführen.</span><span class="sxs-lookup"><span data-stu-id="3529e-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="3529e-107">Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräte Registrierungen verwalten.</span><span class="sxs-lookup"><span data-stu-id="3529e-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="3529e-108">Wenn Sie automatische Registrierungen in Ihrer lokalen Active Directory einrichten, müssen Sie außerdem Administrator von Active Directory und AD FS sein (falls zutreffend).</span><span class="sxs-lookup"><span data-stu-id="3529e-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="3529e-109">Für den Prozess der Hybriden Azure AD Beitritts Registrierung müssen sich Geräte im Unternehmensnetzwerk befinden.</span><span class="sxs-lookup"><span data-stu-id="3529e-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="3529e-110">Es funktioniert auch über VPN, aber es gibt einige Vorbehalte.</span><span class="sxs-lookup"><span data-stu-id="3529e-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="3529e-111">Wir haben Kunden gehört, die Unterstützung bei der Problembehandlung für den Hybrid-Azure AD Anmeldungsprozess unter Remote-Arbeitsbedingungen benötigen.</span><span class="sxs-lookup"><span data-stu-id="3529e-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="3529e-112">**Cloud-Authentifizierungsumgebung (mit Azure AD Kennworthash Synchronisierung oder Pass-Through-Authentifizierung)**</span><span class="sxs-lookup"><span data-stu-id="3529e-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="3529e-113">Dieser Registrierungs Fluss wird auch als "Synchronisierungs Beitritt" bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="3529e-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="3529e-114">Hier finden Sie eine Aufschlüsselung der Vorgänge während des Registrierungsvorgangs:</span><span class="sxs-lookup"><span data-stu-id="3529e-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="3529e-115">Windows 10 erkennt den Dienstverbindungspunkt-Eintrag (SCP), wenn sich der Benutzer am Gerät anmeldet.</span><span class="sxs-lookup"><span data-stu-id="3529e-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="3529e-116">Das Gerät versucht zunächst, Mandanteninformationen aus dem clientseitigen SCP in der Registrierung [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] abzurufen.</span><span class="sxs-lookup"><span data-stu-id="3529e-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="3529e-117">Weitere Informationen finden Sie unter [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="3529e-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="3529e-118">Wenn ein Fehler auftritt, kommuniziert das Gerät mit lokalem Active Directory, um Mandanteninformationen von SCP zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="3529e-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="3529e-119">Um SCP zu überprüfen, lesen Sie dieses [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="3529e-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="3529e-120">Es wird empfohlen, SCP im Active Directory zu aktivieren und nur clientseitigen SCP für die erste Überprüfung zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="3529e-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="3529e-121">Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich gegen Azure AD zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="3529e-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="3529e-122">Sie können überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann, indem Sie das [Verbindungsskript Test Geräteregistrierung](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)verwenden.</span><span class="sxs-lookup"><span data-stu-id="3529e-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="3529e-123">Windows 10 generiert selbstsigniertes Zertifikat und speichert es unter dem Computerobjekt im lokalen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3529e-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="3529e-124">Dies erfordert eine Sicht auf Domänen Controller.</span><span class="sxs-lookup"><span data-stu-id="3529e-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="3529e-125">Das Geräteobjekt, für das das Zertifikat verwendet wird, wird über Azure AD Connect mit Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="3529e-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="3529e-126">Der Synchronisierungszyklus ist standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration von Azure AD Connect ab.</span><span class="sxs-lookup"><span data-stu-id="3529e-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="3529e-127">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="3529e-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="3529e-128">In dieser Phase sollten Sie das Betreff-Gerät im Status "**Ausstehend**" unter Device Blade of Azure Portal sehen können.</span><span class="sxs-lookup"><span data-stu-id="3529e-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="3529e-129">Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="3529e-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3529e-130">Wenn Sie sich auf VPN befinden und Logoff/Login die Domänen Konnektivität beendet, können Sie die Registrierung manuell auslösen.</span><span class="sxs-lookup"><span data-stu-id="3529e-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="3529e-131">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="3529e-131">To do that:</span></span>
    >
    > <span data-ttu-id="3529e-132">Stellen Sie eine `dsregcmd /join` lokale über Administratoreingabeaufforderung oder Remote über PSExec auf Ihrem PC aus.</span><span class="sxs-lookup"><span data-stu-id="3529e-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="3529e-133">Beispiel: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="3529e-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="3529e-134">Häufige Probleme bei der Registrierung von Azure Active Directory-Geräten finden Sie unter [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="3529e-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
