---
title: DataProtection – Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778192"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlocker-Verschlüsselung mit Intune

Intune Endpoint Protection Policy kann zum Konfigurieren von Bitlocker-Verschlüsselungseinstellungen für Windows-Geräte verwendet werden. Weitere Informationen finden Sie unter [Windows 10-Einstellungen (und höher), um Geräte mit Intune zu schützen.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Zusätzlich zur Endpoint Protection-Richtlinie gibt es auch einen Verschlüsselungsbericht, der eine detailliertere Ansicht des Verschlüsselungsstatus für Geräte bietet. Auf diesen Bericht kann über das Portal "MEM" unter "Geräte  **> Monitor"** und dann unter "Konfiguration" ["Verschlüsselungsbericht" zugegriffen werden.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Wenn Sie feststellen, dass Bitlocker nicht wie erwartet aktiviert werden kann oder das profil, das zum Aktivieren von Bitlocker verwendet wird, einen Fehlerstatus hat, lesen Sie den Verschlüsselungsbericht, um ein besseres Verständnis dafür zu erhalten, warum das Verhalten auftritt.

Weitere Informationen zum Interpretieren des Berichts einschließlich der verschiedenen Verschlüsselungsstatuswerte finden Sie unter Überwachen der [Geräteverschlüsselung mit Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Beachten Sie, dass viele neuere Geräte unter Windows 10 die automatische Bitlockerverschlüsselung unterstützen, die ohne Anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Informationen finden Sie in den folgenden häufig gestellten Fragen.

Informationen zur Behandlung von Bitlockerproblemen finden Sie unter Problembehandlung für [BitLocker-Richtlinien in Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Häufig gestellte Fragen**

F: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?<br>
A: Die Einstellungen in der Intune Endpoint #A0 werden mithilfe des [Bitlocker-CSP implementiert.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nicht alle Editionen oder Builds von Windows unterstützen den Bitlocker-CSP. <br><br>

F: Wie kann Bitlocker auf Geräten aktiviert werden, ohne dass eine Benutzerinteraktion erforderlich ist?<br>
A: Solange die erforderlichen Voraussetzungen erfüllt sind, ist es möglich, bitlocker "Automatische Verschlüsselung" über Intune zu aktivieren. Details zu den Geräteanforderungen und Beispielrichtlinieneinstellungen zum Aktivieren der automatischen Verschlüsselung finden Sie im folgenden Dokument: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist, das die Standardeinstellungen des Betriebssystems für Verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verwendet, löst das Anwenden einer Richtlinie mit anderen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen aus?<br>
A: Nein. Um die neuen Verschlüsselungseinstellungen anzuwenden, muss das Laufwerk zuerst entschlüsselt werden.<br><br>
**Hinweis:** Bei Geräten, die bei Autopilot registriert werden, wird die automatische Verschlüsselung, die während der OOBE erfolgen würde, erst ausgelöst, wenn die Richtlinie von Intune ausgewertet wird, wodurch die richtlinienbasierten Einstellungen an Stelle der Betriebssystemeinstellungen verwendet werden können.
 
F: Wenn ein Gerät als Ergebnis der Anwendung der Intune-Richtlinie verschlüsselt wird, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?<br>
A: Das Entfernen der verschlüsselungsbezogenen Richtlinie führt NICHT zur Entschlüsselung der konfigurierten Laufwerke.
 
F: Warum zeigt die Intune-Kompatibilitätsrichtlinie, dass auf meinem Gerät Bitlocker nicht aktiviert ist, obwohl dies der Grund ist?<br>
A: Die Einstellung "Bitlocker aktiviert" in der Intune-Kompatibilitätsrichtlinie verwendet den Windows Device Health Attestation (DHA)-Client. Dieser Client misst den Gerätestatus nur zur Startzeit. Wenn also ein Gerät nicht neu gestartet wurde, seit die Bitlocker-Verschlüsselung abgeschlossen wurde, wird Bitlocker vom Clientdienst für Dies nicht als aktiv angezeigt.
 
 