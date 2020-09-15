---
title: BitLocker-Wiederherstellungsschlüssel
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685885"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Zugreifen auf BitLocker-Wiederherstellungsschlüssel

Wenn Sie BitLocker-Einstellungen für InTune-Endpunktschutz Richtlinien konfigurieren, können Sie festlegen, ob BitLocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.

Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten auf zwei Arten für einen InTune-Administrator als Teil der Gerätedatensatz Daten auf dem Blade "InTune-Geräte" sichtbar sein:

Geräte – Azure AD Geräte – > "Gerät" oder Geräte – > alle Geräte – > "Gerät" – > Wiederherstellungsschlüssel

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
Wenn das Gerät vor der Registrierung in InTune verschlüsselt wurde, ist der Wiederherstellungsschlüssel möglicherweise dem "Microsoft-Konto" (MSA) zugeordnet, das zum Anmelden beim Gerät während des OOBE-Prozesses verwendet wurde. Wenn dies der Fall ist, sollten beim Zugriff auf  https://onedrive.live.com/recoverykey und bei der Anmeldung mit dieser MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel gespeichert wurden.
 
Wenn das Gerät aufgrund der Konfiguration über eine domänenbasierte Gruppenrichtlinie verschlüsselt wurde, werden die Wiederherstellungsinformationen möglicherweise in der lokalen Active Directory gespeichert.
 

