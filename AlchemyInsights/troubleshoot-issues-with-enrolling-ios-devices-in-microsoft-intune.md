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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problembehandlung bei der Registrierung von iOS-Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben. 
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
- **Gerätedeckel erreicht** Der Benutzer hat mehr Geräte als das Gerätelimit registriert. Überprüfen Sie diese Dokumente, [um ein Gerät zu entfernen oder](https://docs.microsoft.com/intune/devices-wipe) das [Gerätelimit zu ändern.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden. In [diesem Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) finden Sie Anweisungen dazu. 
    
- **Benutzerlizenztyp Ungültig oder Benutzername nicht erkannt:** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente, um eine Lizenz zuzuordnen: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Zusätzliche Ressourcen zur Lösung Ihres Problems:
  
1. Verwenden [Sie das Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere [Informationen finden](https://docs.microsoft.com/intune/help-desk-operators) Sie in diesem Dokument. 
    
2. Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Erfahren Sie, wie Sie iOS-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/ios-enroll)
    

