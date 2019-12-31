---
title: BitLocker-Wiederherstellungsschlüssel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908814"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Zugreifen auf BitLocker-Wiederherstellungsschlüssel

Wenn Sie BitLocker-Einstellungen für InTune-Endpunktschutz Richtlinien konfigurieren, können Sie festlegen, ob BitLocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.

Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten auf zwei Arten für einen InTune-Administrator als Teil der Gerätedatensatz Daten auf dem Blade "InTune-Geräte" sichtbar sein:

Geräte – Azure AD Geräte – #a0 "Gerät" oder Geräte – #a1 alle Geräte – #a2 "Gerät" – #a3 Wiederherstellungsschlüssel

Alternativ können Sie den Wiederherstellungsschlüssel (Password) sehen, indem Sie den folgenden Befehl an einer Eingabeaufforderung mit erhöhten Rechten ausführen, wenn ein Administratorzugriff auf das Gerät selbst vorliegt:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Wenn das Gerät vor der Registrierung in InTune verschlüsselt wurde, ist der Wiederherstellungsschlüssel möglicherweise dem "Microsoft-Konto" (MSA) zugeordnet, das zum Anmelden beim Gerät während des OOBE-Prozesses verwendet wurde. Wenn dies der Fall ist, sollten https://onedrive.live.com/recoverykey beim Zugriff auf und bei der Anmeldung mit dieser MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel gespeichert wurden.
 
Wenn das Gerät aufgrund der Konfiguration über eine domänenbasierte Gruppenrichtlinie verschlüsselt wurde, werden die Wiederherstellungsinformationen möglicherweise in der lokalen Active Directory gespeichert.
 

