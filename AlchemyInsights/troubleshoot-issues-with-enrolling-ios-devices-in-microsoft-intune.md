---
title: Behandeln von Problemen beim Registrieren von IOS-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506962"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="a7bbf-102">Behandeln von Problemen beim Registrieren von IOS-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="a7bbf-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="a7bbf-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="a7bbf-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="a7bbf-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="a7bbf-105">**Geräteabdeckung erreicht** Der Benutzer hat mehr Geräte registriert als die Geräte Grenze.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a7bbf-106">Überprüfen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a7bbf-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="a7bbf-107">**Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="a7bbf-108">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , um entsprechende Anweisungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="a7bbf-109">**Benutzer Lizenztyp ungültig oder Benutzer Name nicht erkannt:** Dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="a7bbf-110">Überprüfen Sie diese Dokumente zum Zuweisen einer Lizenz über: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="a7bbf-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="a7bbf-111">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="a7bbf-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a7bbf-112">Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a7bbf-113">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="a7bbf-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="a7bbf-114">Lesen Sie diese Dokumente, um eine Liste der häufigsten Fehler zu finden, die die Registrierung und Auflösungen zu jeder verhindern: [Troubleshooting Guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a7bbf-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="a7bbf-115">[Erfahren Sie, wie Sie IOS-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="a7bbf-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

