---
title: Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830941"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Probleme und Lösungsschritte:
  
 **Fehler "Gerät nicht verschlüsselt" im Unternehmensportal:** Neuere Versionen von Android, insbesondere ab v7.0, erfordern eine Startkennung, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist. Häufige Lösungen sind das Aktivieren eines Startpins oder das vollständige Verschlüsseln des Geräts. Weitere [Informationen finden](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) Sie in diesem Dokument.
  
 Geräte können nicht mit dem Intune-Dienst einchecken oder in der Intune-Verwaltungskonsole als **"Fehlerhaft" anzeigen:** Einige Geräte von Samsung 4.4 und 5.5 checken möglicherweise nicht in den Dienst ein. Es gibt 3 mögliche Lösungen für dieses Problem:
  
1. Öffnen Sie manuell die Intune Company Portal-App, die automatisch eine Gerätesynchronisierung initiiert.

2. Aktualisieren Sie das Gerät auf Android 6.0 oder höher.

3. Deaktivieren Sie den Samsung Smart Manager von der Verwaltung des Intune-Unternehmensportals. Weitere [Informationen zu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) diesen Problemen und Lösungen finden Sie in diesem Dokument.

 **Fehler "Benutzerlizenztyp Ungültig"** oder "Benutzername **nicht erkannt":** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente, um eine Lizenz zuzuordnen: Office Admin Center oder Azure Portal.
  
Zusätzliche Ressourcen zur Lösung Ihres Problems:
  
1. Verwenden [Sie das Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere [Informationen finden](https://docs.microsoft.com/intune/help-desk-operators) Sie in diesem Dokument.

2. In [diesem Dokument finden](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Sie eine Liste der häufigen Fehler, die die Registrierung und Die Lösung der einzelnen Fehler verhindern.

3. [Erfahren Sie, wie Sie Android-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/android-enroll)
