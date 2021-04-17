---
title: DataProtection – Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815614"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlockerverschlüsselung mit Intune

Intune Endpoint Protection Policy kann zum Konfigurieren von Bitlocker-Verschlüsselungseinstellungen für Windows-Geräte verwendet werden. Weitere Informationen finden Sie unter [Windows 10 -Einstellungen (und höher), um Geräte mithilfe von Intune zu schützen.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Zusätzlich zur Endpoint Protection-Richtlinie gibt es auch einen Verschlüsselungsbericht, der eine ausführlichere Ansicht des Verschlüsselungsstatus für Geräte bietet. Auf diesen Bericht kann über das MEM-Portal unter **Geräte > Monitor** zugegriffen werden, und wählen Sie dann unter **Konfiguration** [Verschlüsselungsbericht aus.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Wenn Sie feststellen, dass Bitlocker nicht wie erwartet aktiviert werden kann oder das Profil, das zum Aktivieren von Bitlocker verwendet wird, einen Fehlerstatus hat, lesen Sie bitte den Verschlüsselungsbericht, um ein besseres Verständnis dafür zu erhalten, warum das Verhalten auftritt.

Weitere Informationen zur Interpretation des Berichts einschließlich der verschiedenen Verschlüsselungsstatuswerte finden Sie unter [Überwachen der Geräteverschlüsselung mit Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Beachten Sie, dass viele neuere Geräte unter Windows 10 die automatische Bitlockerverschlüsselung unterstützen, die ohne die Anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung der Richtlinie auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Informationen finden Sie in den folgenden HÄUFIG GESTELLTEN FRAGEN.

Informationen zur Problembehandlung von Bitlockerproblemen finden Sie unter [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Häufig gestellte Fragen**

F: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?<br>
A: Die Einstellungen in intune Endpoint Protection Policy werden mit dem [Bitlocker CSP implementiert.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nicht alle Editionen oder Builds von Windows unterstützen den Bitlocker CSP. <br><br>

F: Wie kann Bitlocker auf Geräten aktiviert werden, ohne dass eine Endbenutzerinteraktion erforderlich ist?<br>
A: Solange die erforderlichen Voraussetzungen erfüllt sind, ist es möglich, Bitlocker "Silent Encryption" über Intune zu aktivieren. Weitere Informationen zu den Geräteanforderungen und Beispielrichtlinieneinstellungen zum Aktivieren der automatischen Verschlüsselung finden Sie im folgenden Dokument: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist, indem die Standardeinstellungen des Betriebssystems für Verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verwendet werden, löst das Anwenden einer Richtlinie mit anderen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen aus?<br>
A: Nein. Zum Anwenden der neuen Verschlüsselungseinstellungen muss das Laufwerk zunächst entschlüsselt werden.<br><br>
**Hinweis:** Bei Geräten, die bei Autopilot registriert werden, wird die automatische Verschlüsselung, die während der OOBE auftreten würde, erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, wodurch die richtlinienbasierten Einstellungen an Stelle der Standardeinstellungen des Betriebssystems verwendet werden können.
 
F: Wenn ein Gerät durch die Anwendung der Intune-Richtlinie verschlüsselt wird, wird es dann entschlüsselt, wenn diese Richtlinie entfernt wird?<br>
A: Das Entfernen verschlüsselungsbezogener Richtlinien führt NICHT zur Entschlüsselung der konfigurierten Laufwerke.
 
F: Warum zeigt intune Compliance Policy, dass auf meinem Gerät Bitlocker nicht aktiviert ist, obwohl es dies ist?<br>
A: Die Einstellung "Bitlocker aktiviert" in der Intune-Kompatibilitätsrichtlinie verwendet den Windows Device Health Attestation (DHA)-Client. Dieser Client misst nur den Gerätestatus zum Startzeit. Wenn also ein Gerät seit Abschluss der Bitlockerverschlüsselung nicht neu gestartet wurde, wird Bitlocker vom DHA-Clientdienst nicht als aktiv angezeigt.
 
 