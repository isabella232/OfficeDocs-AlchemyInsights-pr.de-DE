---
title: Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft Intune
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708889"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0a9e6-102">Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0a9e6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0a9e6-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="0a9e6-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="0a9e6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0a9e6-105">**Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="0a9e6-106">Laden Sie das PC-Client-Softwarepaket erneut in der Intune Admin Console herunter.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="0a9e6-107">Weitere Informationen finden Sie in dieser Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="0a9e6-108">**Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:</span><span class="sxs-lookup"><span data-stu-id="0a9e6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="0a9e6-109">Der Benutzer hat mehr Geräte als das Gerätelimit registriert.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0a9e6-110">Überprüfen Sie diese Dokumente, [um ein Gerät zu entfernen oder](https://docs.microsoft.com/intune/devices-wipe) das [Gerätelimit zu ändern.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="0a9e6-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="0a9e6-111">"Benutzer können Geräte zu Azure AD beitreten" ist auf "keine" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="0a9e6-112">Legen Sie es auf alle Benutzer oder wählen Sie Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-112">Set it to all or select users.</span></span> <span data-ttu-id="0a9e6-113">Weitere [Informationen finden](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) Sie in dieser Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="0a9e6-114">Das Gerät wurde bereits von einem anderen Benutzer registriert.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="0a9e6-115">Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure Intune-Konsole, oder entrollen Sie das Gerät manuell, bevor Sie es erneut versuchen.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="0a9e6-116">Das Gerät ist Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="0a9e6-117">Nur Windows 10 Pro-, Education- und Enterprise-SKUs können Azure Active Directory beitreten.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="0a9e6-118">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="0a9e6-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="0a9e6-119">Verwenden [Sie das Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0a9e6-120">Weitere [Informationen finden](https://docs.microsoft.com/intune/help-desk-operators) Sie in diesem Dokument.</span><span class="sxs-lookup"><span data-stu-id="0a9e6-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="0a9e6-121">Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0a9e6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="0a9e6-122">[Erfahren Sie, wie Sie Windows-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="0a9e6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
