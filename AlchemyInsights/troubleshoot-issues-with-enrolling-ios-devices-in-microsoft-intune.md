---
title: Behandeln von Problemen beim Registrieren von IOS-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669247"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="82a59-102">Behandeln von Problemen beim Registrieren von IOS-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="82a59-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="82a59-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="82a59-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="82a59-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="82a59-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="82a59-105">**Geräteabdeckung erreicht** Der Benutzer hat mehr Geräte registriert als die Geräte Grenze.</span><span class="sxs-lookup"><span data-stu-id="82a59-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="82a59-106">Überprüfen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="82a59-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="82a59-107">**Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden.</span><span class="sxs-lookup"><span data-stu-id="82a59-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="82a59-108">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , um entsprechende Anweisungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="82a59-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="82a59-109">**Benutzer Lizenztyp ungültig oder Benutzer Name nicht erkannt:** Dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="82a59-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="82a59-110">Überprüfen Sie diese Dokumente zum Zuweisen einer Lizenz über: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="82a59-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="82a59-111">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="82a59-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="82a59-112">Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="82a59-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="82a59-113">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="82a59-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="82a59-114">Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="82a59-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="82a59-115">[Erfahren Sie, wie Sie IOS-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="82a59-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

