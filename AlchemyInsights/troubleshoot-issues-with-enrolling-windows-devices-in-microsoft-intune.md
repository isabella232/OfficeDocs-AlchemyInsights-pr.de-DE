---
title: Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390642"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft InTune

Lesen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben. 
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
 **Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen. Laden Sie das PC-Client-Softwarepaket in der InTune-Verwaltungskonsole erneut herunter. Weitere Informationen finden Sie in dieser Dokumentation. 
  
 **Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten: 
  
1. Der Benutzer hat mehr Geräte als der Geräte Grenzwert registriert. Lesen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Benutzer können Geräte mit Azure AD verbinden" ist auf "None" festgelegt. Legen Sie Sie auf alle oder Benutzer auswählen fest. Weitere Informationen finden Sie in [dieser Dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) . 
    
3. Das Gerät ist bereits von einem anderen Benutzer registriert. Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure InTune-Konsole, oder heben Sie die Registrierung des Geräts auf, bevor Sie es erneut versuchen.
    
4. Das Gerät ist Windows 10 Home. Nur Windows 10 pro, Education und Enterprise-SKUs können Azure Active Directory beitreten.
    
Weitere Ressourcen zur Lösung des Problems:
  
1. Verwenden Sie [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) zur Diagnose und Lösung allgemeiner Registrierungsfehler. Weitere Informationen finden Sie in [diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Sehen Sie sich diese Dokumente an, um eine Liste allgemeiner Fehler zu finden, die die Registrierung und Auflösungen für jedes Dokument verhindern: [Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlung](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Erfahren Sie, wie Sie Windows-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/windows-enroll).
  

