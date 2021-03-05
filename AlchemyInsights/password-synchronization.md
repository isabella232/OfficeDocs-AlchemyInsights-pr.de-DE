---
title: Kennwortsynchronisierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449140"
---
# <a name="password-synchronization"></a><span data-ttu-id="7dc48-102">Kennwortsynchronisierung</span><span class="sxs-lookup"><span data-stu-id="7dc48-102">Password synchronization</span></span>

<span data-ttu-id="7dc48-103">**Kennworthashsynchronisierung funktioniert überhaupt nicht**</span><span class="sxs-lookup"><span data-stu-id="7dc48-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="7dc48-104">Einige häufige Probleme, die Kunden auftreten, wenn die Kennworthashsynchronisierung nicht funktioniert, sind:</span><span class="sxs-lookup"><span data-stu-id="7dc48-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="7dc48-105">Das active Directory-Konto, das von Azure AD Connect für  die Kommunikation mit lokalem Active Directory verwendet wird, erhält keine Replikation von Verzeichnisänderungen und Verzeichnisänderungen **Replizieren Alle** Berechtigungen, die für die Kennwortsynchronisierung erforderlich sind. Sie müssen dies beheben, indem Sie dem Active Directory-Konto diese Berechtigungen erteilen.</span><span class="sxs-lookup"><span data-stu-id="7dc48-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="7dc48-106">Die Kennworthashsynchronisierung wird deaktiviert, nachdem ein  Administrator die User Sign-In-Methode von der Kennwortsynchronisierung in eine andere Option wie  den Verbund mit **AD FS** im Azure AD Sign-In geändert hat. Sie können dies beheben, indem Sie das Feature für die Kennworthashsynchronisierung im Azure AD #A1 erneut aktivieren.</span><span class="sxs-lookup"><span data-stu-id="7dc48-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="7dc48-107">Verbindungsproblem mit lokalem Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7dc48-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="7dc48-108">Beispielsweise kann azure AD Connect nicht auf einige [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Domänencontroller zugreifen, oder die erforderlichen Ports werden von der Firewall blockiert. Sie müssen dies beheben, indem Sie sicherstellen, dass die Verbindung zwischen dem Azure AD Connect-Server und dem lokalen Active Directory ordnungsgemäß funktioniert.</span><span class="sxs-lookup"><span data-stu-id="7dc48-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="7dc48-109">Azure AD #A0 befindet sich derzeit im Stagingmodus, was dazu führt, dass der Server nicht in der Lage ist, die Kennworthashes zu verwenden. Führen Sie zur Problembehandlung die im Abschnitt Problembehandlung bei der Kennwortsynchronisierung mit azure AD Connect-Synchronisierung beschriebenen Schritte aus: Keine Kennwörter werden [synchronisiert.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="7dc48-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="7dc48-110">**Kennworthashsynchronisierung funktioniert für einige meiner Benutzer nicht**</span><span class="sxs-lookup"><span data-stu-id="7dc48-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="7dc48-111">Wenn Sie festgestellt haben, dass der Kennworthash  für einen Benutzer nicht synchronisiert wird, verwenden Sie die Problembehandlungsaufgabe in Azure AD Connect, um das Problem zu untersuchen und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="7dc48-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="7dc48-112">Führen Sie die folgenden Aufgaben aus:</span><span class="sxs-lookup"><span data-stu-id="7dc48-112">Perform the following tasks:</span></span>

    <span data-ttu-id="7dc48-113">a.</span><span class="sxs-lookup"><span data-stu-id="7dc48-113">a.</span></span> [<span data-ttu-id="7dc48-114">Ausführen der Problembehandlungsaufgabe im Assistenten</span><span class="sxs-lookup"><span data-stu-id="7dc48-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="7dc48-115">b.</span><span class="sxs-lookup"><span data-stu-id="7dc48-115">b.</span></span> [<span data-ttu-id="7dc48-116">Verwenden des Cmdlets zur Problembehandlung, um das Problem der Kennworthashsynchronisierung für eine bestimmte Verwendung zu untersuchen</span><span class="sxs-lookup"><span data-stu-id="7dc48-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="7dc48-117">Das lokale Active Directory User-Objekt ist für Benutzer aktiviert, um das Kennwort bei der **nächsten Anmeldeoption zu** ändern.</span><span class="sxs-lookup"><span data-stu-id="7dc48-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="7dc48-118">Wenn diese Option aktiviert ist, wird dem Benutzer ein temporäres Kennwort zugewiesen, und er wird aufgefordert, das Kennwort bei der nächsten Anmeldung zu ändern.</span><span class="sxs-lookup"><span data-stu-id="7dc48-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="7dc48-119">Azure AD Connect synchronisiert keine temporären Kennwörter mit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7dc48-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="7dc48-120">Führen Sie eine der folgenden Aufgaben aus, um das oben beschriebene Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="7dc48-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="7dc48-121">Bitten Sie den Benutzer, sich bei der lokalen Anwendung (z. B. Windows Desktop) zu anmelden und das Kennwort zu ändern.</span><span class="sxs-lookup"><span data-stu-id="7dc48-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="7dc48-122">Das neue Kennwort wird mit Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="7dc48-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="7dc48-123">Ein Administrator muss das Kennwort des Benutzers aktualisieren, ohne die Option Benutzer muss das Kennwort bei der nächsten Anmeldung ändern **und** das neue Kennwort für den Benutzer freigeben.</span><span class="sxs-lookup"><span data-stu-id="7dc48-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="7dc48-124">Das lokale Active Directory User-Objekt ist **nicht ordnungsgemäß** für die Objektsynchronisierung oder Kennwortsynchronisierung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="7dc48-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="7dc48-125">Um dieses Problem zu beheben, führen Sie die unter Problembehandlung der Kennworthashsynchronisierung mit [Azure AD Connect-Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)beschriebenen Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="7dc48-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







