---
title: Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420591"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft InTune

Lesen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Probleme und Lösungsschritte:
  
 **Fehler beim nicht VerschlüsselTen Gerät im Unternehmens Portal:** Neuere Versionen von Android, insbesondere ab v 7.0, erfordern einen startpasscode, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist. Gängige Lösungen sind die Aktivierung einer Start-PIN oder das vollständige Verschlüsseln des Geräts. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , um weitere Informationen zu erhalten. 
  
 **Geräte können nicht mit dem InTune-Dienst Einchecken oder als "fehlerhaft" in der InTune-Verwaltungskonsole angezeigt werden:** Einige Samsung 4,4-und 5,5-Geräte können nicht in den Dienst einchecken. Es gibt drei mögliche Lösungen für dieses Problem: 
  
1. Öffnen Sie die Intune-Unternehmens Portal-APP, die automatisch eine Gerätesynchronisierung initiiert.
    
2. Aktualisieren Sie das Gerät auf Android 6,0 oder höher.
    
3. Deaktivieren Sie Samsung Smart Manager aus der Verwaltung des InTune-Unternehmensportals. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , um weitere Informationen zu diesen Problemen und Lösungen zu finden. 
    
 **Benutzer lizenzTyp ungültig** oder **Benutzer Name nicht erkannt Fehler:** dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen sein. Lesen Sie diese Dokumente zum Zuweisen einer Lizenz über: Office Admin Center oder Azure Portal. 
  
Weitere Ressourcen zur Lösung des Problems:
  
1. Verwenden Sie [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) zur Diagnose und Lösung allgemeiner Registrierungsfehler. Weitere Informationen finden Sie in [diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. In [diesem Dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) finden Sie eine Liste häufig auftretender Fehler, die die Registrierung und die Auflösungen verhindern. 
    
3. [Erfahren Sie, wie Sie Android-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/android-enroll).
    

