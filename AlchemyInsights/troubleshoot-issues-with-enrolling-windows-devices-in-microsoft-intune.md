---
title: Behandeln von Problemen mit der Registrierung von Windows-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353536"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Behandeln von Problemen mit der Registrierung von Windows-Geräten in Microsoft InTune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
 **Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen. Laden Sie das PC-Client-Softwarepaket in der InTune-Verwaltungskonsole erneut herunter. Lesen Sie diese Dokumentation, um weitere Informationen zu erhalten.
  
 **Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:
  
1. Der Benutzer hat mehr Geräte registriert als die Geräte Grenze. Überprüfen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Benutzer können Geräte zu Azure AD hinzufügen" ist auf "None" festgelegt. Legen Sie ihn auf alle fest, oder wählen Sie Benutzer aus. Lesen Sie [Diese Dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , um weitere Informationen zu erhalten.

3. Das Gerät ist bereits von einem anderen Benutzer registriert. Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure InTune-Konsole, oder heben Sie die Registrierung des Geräts manuell auf, bevor Sie es erneut versuchen.

4. Das Gerät ist Windows 10 Home. Nur Windows 10 pro, Education und Enterprise-SKUs können Azure Active Directory beitreten.

Zusätzliche Ressourcen zur Lösung Ihres Problems:
  
1. Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren.

2. Lesen Sie diese Dokumente, um eine Liste der häufigsten Fehler zu finden, die die Registrierung und Auflösungen zu jeder verhindern: [Troubleshooting Guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Erfahren Sie, wie Sie Windows-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/windows-enroll).
