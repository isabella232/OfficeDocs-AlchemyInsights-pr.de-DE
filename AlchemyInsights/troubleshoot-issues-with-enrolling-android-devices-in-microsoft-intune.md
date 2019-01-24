---
title: Behandeln von Problemen mit Android-Geräte in Microsoft Intune registrieren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469926"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Behandeln von Problemen mit Android-Geräte in Microsoft Intune registrieren

Überprüfen Sie die unten aufgeführten Ressourcen zur Lösung des Problems jetzt.
  
Häufige Probleme und Lösungsschritte:
  
 **Gerät nicht verschlüsselt Fehler im Unternehmensportal:** Sobald neuere Versionen von Android, insbesondere beginnend mit Version 7.0, erforderlich zum Starten des Kennung dafür sorgen, dass Ihr Gerät vollständig verschlüsselt ist. Häufig sind, aktivieren eine Pin zum Starten des oder das Gerät vollständig zu verschlüsseln. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) Weitere Informationen. 
  
 **Nicht Geräten erkundigen Sie sich bei dem Intune-Dienst oder als "Fehlerhaft" in der Verwaltungskonsole Intune anzeigen:** Einige Samsung 4.4 und 5.5 Geräte möglicherweise nicht in den Dienst überprüft. Es gibt 3 Lösungsvorschläge für dieses Problem: 
  
1. Öffnen Sie manuell die Intune Unternehmensportal-app, die automatisch eine Synchronisierung Gerät wird initiiert.
    
2. Aktualisieren Sie das Gerät auf Android 6.0 oder höher.
    
3. Verwalten von der Intune Unternehmensportal deaktivieren Sie Samsung Smart-Manager. [In diesem Dokument](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) Weitere Informationen zu diesen Problemen und Lösungen überprüfen. 
    
 **Benutzer Lizenz Typ ungültig** oder **Fehler Benutzer Name nicht erkannt:** der Benutzer eine Lizenz Intune oder zur Abstimmung zugewiesen werden soll. Lesen Sie diese Dokumente über eine Lizenz zuweisen: Office-Verwaltungskonsole oder Azure-Portal. 
  
Zusätzliche Ressourcen zu Ihrem Problem zu beheben:
  
1. Mithilfe von [Intune Problembehandlung Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostizieren und Beheben von häufig auftretenden Fehler der Registrierung. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) für weitere Details. 
    
2. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) für eine Liste mit häufigen Fehlern, die Registrierung und Auflösung für jeden zu verhindern. 
    
3. [Erfahren Sie, wie in Microsoft Intune Android-Geräte zu registrieren](https://docs.microsoft.com/en-us/intune/android-enroll).
    

