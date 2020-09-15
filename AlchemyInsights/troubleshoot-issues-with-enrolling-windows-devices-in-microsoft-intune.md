---
title: Behandeln von Problemen mit der Registrierung von Windows-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658877"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="dd8e8-102">Behandeln von Problemen mit der Registrierung von Windows-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="dd8e8-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="dd8e8-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="dd8e8-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="dd8e8-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="dd8e8-105">**Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="dd8e8-106">Laden Sie das PC-Client-Softwarepaket in der InTune-Verwaltungskonsole erneut herunter.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="dd8e8-107">Lesen Sie diese Dokumentation, um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="dd8e8-108">**Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:</span><span class="sxs-lookup"><span data-stu-id="dd8e8-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="dd8e8-109">Der Benutzer hat mehr Geräte registriert als die Geräte Grenze.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="dd8e8-110">Überprüfen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="dd8e8-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="dd8e8-111">"Benutzer können Geräte zu Azure AD hinzufügen" ist auf "None" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="dd8e8-112">Legen Sie ihn auf alle fest, oder wählen Sie Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-112">Set it to all or select users.</span></span> <span data-ttu-id="dd8e8-113">Lesen Sie [Diese Dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="dd8e8-114">Das Gerät ist bereits von einem anderen Benutzer registriert.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="dd8e8-115">Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure InTune-Konsole, oder heben Sie die Registrierung des Geräts manuell auf, bevor Sie es erneut versuchen.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="dd8e8-116">Das Gerät ist Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="dd8e8-117">Nur Windows 10 pro, Education und Enterprise-SKUs können Azure Active Directory beitreten.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="dd8e8-118">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="dd8e8-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="dd8e8-119">Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="dd8e8-120">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="dd8e8-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="dd8e8-121">Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="dd8e8-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="dd8e8-122">[Erfahren Sie, wie Sie Windows-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="dd8e8-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
