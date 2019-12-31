---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908709"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der BitLocker-Verschlüsselung mit InTune

 Die Intune-Endpunktschutz Richtlinie kann zum Konfigurieren von BitLocker-Verschlüsselungseinstellungen für Windows-Geräte verwendet werden. Weitere Informationen finden Sie unter [Einstellungen für Windows 10 (und höher), um Geräte mit InTune zu schützen](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Beachten Sie, dass viele neuere Geräte mit Windows 10 die automatische BitLocker-Verschlüsselung unterstützen, die ohne Anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht standardmäßige Einstellungen konfiguriert werden. Weitere Informationen finden Sie in den folgenden FAQ.
 
Informationen zur Behandlung von BitLocker-Problemen finden Sie unter [Problembehandlung für BitLocker-Richtlinien in Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Häufig gestellte Fragen**

 F.: welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpunktschutz Richtlinie?<br>
 A.: die Einstellungen in der InTune-Endpunktschutz Richtlinie werden mithilfe des [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)implementiert. Nicht alle Editionen oder Builds von Windows unterstützen den BitLocker-CSP. <br><br>
      Zu diesem Zeitpunkt werden die folgenden Windows-Editionen unterstützt: Enterprise, Education, Mobile, Mobile Enterprise und Professional (Build 1809 und höher).
 
F.: Wenn ein Gerät bereits mit BitLocker mit den Standardeinstellungen für Verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verschlüsselt ist, wird durch die Anwendung einer Richtlinie mit unterschiedlichen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?<br>
A.: Nein. Damit die neuen Verschlüsselungseinstellungen angewendet werden, muss das Laufwerk zunächst entschlüsselt werden.<br><br>
**Hinweis:** Für Geräte, die mit Autopilot registriert werden, wird die automatische Verschlüsselung, die während der OOBE erfolgen würde, erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, sodass die richtlinienbasierten Einstellungen anstelle der Standardwerte für das Betriebssystem verwendet werden können.
 
F.: wird ein Gerät aufgrund der Anwendung der InTune-Richtlinie verschlüsselt, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?<br>
A: das Entfernen einer Verschlüsselungs bezogenen Richtlinie führt nicht zur Entschlüsselung der konfigurierten Laufwerke.
 
F: Warum zeigt die Intune-Konformitätsrichtlinie an, dass für mein Gerät BitLocker nicht aktiviert ist, obwohl dies der Fall ist?<br>
A.: die Einstellung "BitLocker Enabled" in der InTune-Konformitätsrichtlinie verwendet den Windows-Client für Geräte Integritäts Bescheinigung (DHA). Dieser Client misst nur den Gerätestatus zum Zeitpunkt des Bootens. Wenn also ein Gerät seit der BitLocker-Verschlüsselung nicht neu gestartet wurde, meldet der DHA-Client Dienst BitLocker nicht als aktiv.
 
 