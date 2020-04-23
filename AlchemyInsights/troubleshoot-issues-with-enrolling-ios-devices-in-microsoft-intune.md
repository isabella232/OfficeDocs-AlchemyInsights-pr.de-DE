---
title: Behandeln von Problemen beim Registrieren von IOS-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736157"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Behandeln von Problemen beim Registrieren von IOS-Geräten in Microsoft InTune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben. 
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
- **Geräteabdeckung erreicht** Der Benutzer hat mehr Geräte registriert als die Geräte Grenze. Überprüfen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , um entsprechende Anweisungen zu erhalten. 
    
- **Benutzer Lizenztyp ungültig oder Benutzer Name nicht erkannt:** Dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente zum Zuweisen einer Lizenz über: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Zusätzliche Ressourcen zur Lösung Ihres Problems:
  
1. Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren. 
    
2. Lesen Sie diese Dokumente, um eine Liste der häufigsten Fehler zu finden, die die Registrierung und Auflösungen zu jeder verhindern: [Troubleshooting Guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Erfahren Sie, wie Sie IOS-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/ios-enroll).
    

