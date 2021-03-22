---
title: Ich werde durch den bedingten Zugriff mit einem in der Domäne eingebunden Gerät blockiert
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965464"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="fcc9f-102">Ich werde durch den bedingten Zugriff mit einem in der Domäne eingebunden Gerät blockiert</span><span class="sxs-lookup"><span data-stu-id="fcc9f-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="fcc9f-103">**Sehr empfehlenswerte Tools**</span><span class="sxs-lookup"><span data-stu-id="fcc9f-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="fcc9f-104">[Problembehandlungstool für Geräteregistrierungen](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Ein Tool zur Behebung der häufigsten Probleme bei der Geräteregistrierung.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="fcc9f-105">[Skript zum Testen der Verbindung der Geräteregistrierung](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Ein Skript, mit dem sichergestellt wird, dass ein Gerät unter dem Systemkonto auf Endpunkte der Geräteregistrierung zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="fcc9f-106">[Azure AD-Gerätebereinigungsskript](https://github.com/mzmaili/AzureADDeviceCleanup) – Ein Skript, um veraltete Geräte in Ihrer Umgebung aufzufinden und zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="fcc9f-107">Hier finden Sie einige häufige Ursachen, warum der bedingte Zugriff bei einem Gerät, das in einer Domäne eingebunden ist, (Azure AD Hybrid), fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="fcc9f-108">**Es gibt kein Azure AD-PRT auf dem Gerät** – Sie müssen sicherstellen, dass das Gerät über das primäre Azure AD-Aktualisierungstoken (PRT) verfügt.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="fcc9f-109">Weitere Informationen zu PRT finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="fcc9f-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="fcc9f-110">Um zu überprüfen, ob Sie über das Azure AD-PRT verfügen, können Sie den `dsregcmd/status`-Befehl auf dem Gerät ausführen. Überprüfen Sie, ob „AzureAdPrt“ gleich „JA“ ist.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="fcc9f-111">Wenn „AzureAdPrt“ gleich „NEIN“ ist, überprüfen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="fcc9f-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="fcc9f-112">**Unabhängig davon, ob Sie über eine Verbundumgebung mit ADFS verfügen und diese von den Heimnetzwerken Ihrer Benutzer nicht erreichbar ist**: Stellen Sie in diesem Fall sicher, dass über das Extranet auf Ihre „usernamemixed“-Endpunkte zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="fcc9f-113">Wenn sich Ihre ADFS hinter einem VPN befinden, stellen Sie sicher, dass sich die Benutzer mit dem VPN verbinden und sich erneut auf dem Gerät anmelden.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="fcc9f-114">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="fcc9f-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="fcc9f-115">**Führen Sie Folgendes durch, wenn das TPM des Geräts fehlerhaft ist und es daher nicht authentifiziert werden kann**: Überprüfen Sie „tpm.msc“, um herauszufinden, ob der Status von TPM „Bereit“ ist.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="fcc9f-116">Falls dies nicht der Fall ist, führen Sie den Befehl `dsregcmd/leave` aus, und lassen Sie das Gerät wieder mit Azure AD verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="fcc9f-117">Führen Sie den Vorgang anschließend erneut aus.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-117">Then, try again.</span></span> <span data-ttu-id="fcc9f-118">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="fcc9f-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="fcc9f-119">**Sie verwenden einen Identitätsanbieter eines Drittanbieters, der das WS-Trust-Protokoll nicht unterstützt**.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="fcc9f-120">Wie in unseren Dokumenten beschrieben, können mit Azure AD Hybrid verbundene Geräte in diesem Fall nicht funktionieren.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="fcc9f-121">Wenden Sie sich an Ihren Identitätsanbieter, um Unterstützung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="fcc9f-122">**Benutzer verwenden den Chrome-Browser ohne die Windows 10-Konten** oder **Office-Erweiterung; Chrome verwendet den PRT nicht automatisch bei mit AAD oder AAD Hybrid verbundenen Geräten**: Dies führt zu einem Fehler bei allen gerätebasierten Richtlinien für den bedingten Zugriff, und die Fehlermeldung „Nicht registriertes Gerät“ wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="fcc9f-123">Damit Sie den Chrome-Browser ordnungsgemäß verwenden können, müssen Sie die „Windows 10-Konten“ oder die „Office-Erweiterung des Chrome-Browsers der Benutzer“ über den SCCM oder Intune installieren.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="fcc9f-124">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="fcc9f-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="fcc9f-125">Wenn es nicht möglich ist, die Erweiterung remote zu übertragen, benachrichtigen Sie die Benutzer, eine der oben genannten Erweiterungen manuell zu installieren, um hinter dem gerätebasierten bedingten Zugriff auf Anwendungen zu zugreifen.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="fcc9f-126">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="fcc9f-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="fcc9f-127">**Das Gerät war ordnungsgemäß in Azure AD Hybrid eingebunden, wurde aber versehentlich gelöscht oder deaktiviert, entweder aufgrund von Synchronisierungsänderungen in Azure AD Connect oder über das Azure-Portal**: In diesem Fall wird das Geräteobjekt nicht mehr als vollständig eingebundenes Gerät erkannt, obwohl die Status „AzureAdJoined“ und „PRT“ auf dem Gerät als gültig angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="fcc9f-128">Um dieses Problem zu beheben, führen Sie den `dsregcmd/leave`-Befehl auf den betroffenen Geräten aus, und lassen Sie sie wieder mit Azure AD verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="fcc9f-129">Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="fcc9f-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="fcc9f-130">Wenn Ihre Geräte unter Windows 10, Version 1809, mit VPN/Cloud-Proxy laufen und Probleme mit dem Status „AzureAdPrt“ oder bei einer beliebigen App Probleme mit SSO auftreten (Outlook konnte keine Verbindung mit Postfach herstellen, obwohl PRT verwendet wurde), stellen Sie sicher, dass Sie über dieses Patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) oder das kumulative April-Update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) verfügen, um PRT-Fehler auf diesen Geräten zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="fcc9f-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















