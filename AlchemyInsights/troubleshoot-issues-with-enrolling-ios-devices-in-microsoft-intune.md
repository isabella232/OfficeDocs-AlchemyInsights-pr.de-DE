---
title: Behandeln von Problemen bei der Registrierung von iOS-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391006"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="7aeb0-102">Behandeln von Problemen bei der Registrierung von iOS-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="7aeb0-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="7aeb0-103">Lesen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="7aeb0-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="7aeb0-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="7aeb0-105">**Gerätedeckel erreicht** Der Benutzer hat mehr Geräte als der Geräte Grenzwert registriert.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7aeb0-106">Lesen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="7aeb0-107">**Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** der Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="7aeb0-108">In [diesem Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) finden Sie Anweisungen dazu.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="7aeb0-109">**Benutzer lizenzTyp ungültig oder Benutzer Name nicht erkannt:** Dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="7aeb0-110">Lesen Sie diese Dokumente zum Zuweisen einer Lizenz über: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="7aeb0-111">Weitere Ressourcen zur Lösung des Problems:</span><span class="sxs-lookup"><span data-stu-id="7aeb0-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7aeb0-112">Verwenden Sie [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) zur Diagnose und Lösung allgemeiner Registrierungsfehler.</span><span class="sxs-lookup"><span data-stu-id="7aeb0-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7aeb0-113">Weitere Informationen finden Sie in [diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="7aeb0-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="7aeb0-114">Sehen Sie sich diese Dokumente an, um eine Liste allgemeiner Fehler zu finden, die die Registrierung und Auflösungen für jedes Dokument verhindern: [Problembehandlung](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) und [Problembehandlung](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="7aeb0-115">[Erfahren Sie, wie Sie IOS-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="7aeb0-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

