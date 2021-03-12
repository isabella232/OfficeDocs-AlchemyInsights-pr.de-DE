---
title: Problembehandlung bei der Registrierung von iOS-Geräten in Microsoft Intune
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708961"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="bd3af-102">Problembehandlung bei der Registrierung von iOS-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bd3af-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="bd3af-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="bd3af-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="bd3af-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="bd3af-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="bd3af-105">**Gerätedeckel erreicht** Der Benutzer hat mehr Geräte als das Gerätelimit registriert.</span><span class="sxs-lookup"><span data-stu-id="bd3af-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bd3af-106">Überprüfen Sie diese Dokumente, [um ein Gerät zu entfernen oder](https://docs.microsoft.com/intune/devices-wipe) das [Gerätelimit zu ändern.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="bd3af-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="bd3af-107">**Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden.</span><span class="sxs-lookup"><span data-stu-id="bd3af-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="bd3af-108">In [diesem Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) finden Sie Anweisungen dazu.</span><span class="sxs-lookup"><span data-stu-id="bd3af-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="bd3af-109">**Benutzerlizenztyp Ungültig oder Benutzername nicht erkannt:** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="bd3af-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bd3af-110">Überprüfen Sie diese Dokumente, um eine Lizenz zuzuordnen: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="bd3af-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="bd3af-111">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="bd3af-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bd3af-112">Verwenden [Sie das Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="bd3af-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bd3af-113">Weitere [Informationen finden](https://docs.microsoft.com/intune/help-desk-operators) Sie in diesem Dokument.</span><span class="sxs-lookup"><span data-stu-id="bd3af-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="bd3af-114">Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bd3af-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="bd3af-115">[Erfahren Sie, wie Sie iOS-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="bd3af-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

