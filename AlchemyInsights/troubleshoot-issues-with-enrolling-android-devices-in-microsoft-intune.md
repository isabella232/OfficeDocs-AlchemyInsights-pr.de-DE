---
title: Behandeln von Problemen beim Registrieren von Android-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367288"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Behandeln von Problemen beim Registrieren von Android-Geräten in Microsoft InTune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Probleme und Lösungsschritte:
  
 **Fehler des nicht verschlüsselten Geräts im Unternehmens Portal:** Neuere Versionen von Android, insbesondere ab v 7.0, erfordern eine Startkennung, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist. Häufige Lösungen sind das Aktivieren einer Start-PIN oder das vollständige Verschlüsseln des Geräts. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , um weitere Informationen zu erhalten.
  
 **Geräte können nicht mit dem InTune-Dienst Einchecken oder in der InTune-Verwaltungskonsole als "ungesund" anzeigen:** Einige Geräte von Samsung 4,4 und 5,5 werden möglicherweise nicht in den Dienst eingecheckt. Es gibt drei mögliche Lösungen für dieses Problem:
  
1. Öffnen Sie die Intune-Unternehmens Portal-app manuell, wodurch automatisch eine Gerätesynchronisierung initiiert wird.

2. Aktualisieren Sie das Gerät auf Android 6,0 oder höher.

3. Deaktivieren Sie Samsung Smart Manager für die Verwaltung des InTune-Unternehmensportals. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , um weitere Details zu diesen Problemen und Lösungen zu erfahren.

 Der **Benutzer Lizenztyp ist ungültig** oder der **Benutzer Name wurde nicht erkannt Fehler:** dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente zum Zuweisen einer Lizenz über: Office Admin Center oder Azure Portal.
  
Zusätzliche Ressourcen zur Lösung Ihres Problems:
  
1. Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren.

2. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , um eine Liste der häufigsten Fehler zu finden, die die Registrierung und Auflösungen verhindern.

3. [Erfahren Sie, wie Sie Android-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/android-enroll).
