---
title: Haben Ihre Benutzer bösartige E-Mails empfangen?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291791"
---
# <a name="did-your-users-receive-malicious-email"></a>Haben Ihre Benutzer bösartige e-Mails empfangen?

- Die können bösartige E-Mails jetzt ganz einfach an Microsoft melden, indem Sie die [Administrator-Übermittlungen im Security & Compliance Center](https://sip.protection.office.com/reportsubmission) verwenden.

Nachrichten, die über [Administrator-Übermittlungen](https://sip.protection.office.com/reportsubmission) eingereicht werden, werden überprüft, und die folgenden Ergebnisse werden im Flyout **Details** angezeigt:

- Mögliche Fehler in der E-Mail-Authentifizierung des Absenders zum Zeitpunkt der Auslieferung.
- Informationen zu Richtlinientreffern, welche die Bewertung über einer Nachricht beeinflusst oder überschrieben haben könnten.
- Aktuelle Detonationsergebnisse, um festzustellen, ob die in der Nachricht enthaltenen URLs oder Dateien böswillig waren oder nicht.
- Feedback von Bewertern

Wenn eine Überschreibung gefunden wurde, sollte der erneute Scan in einigen Minuten abgeschlossen sein. Wenn es kein Problem mit der E-Mail-Authentifizierung gab oder die Auslieferung nicht von einer Überschreibung beeinflusst war, dann kann das Feedback der Bewerter bis zu einem Tag dauern.

Wenn Sie mit der endgültigen Bewertung über eine Nachricht, URL oder Datei (blockiert vs. nicht blockiert) nicht einverstanden sind, reichen Sie die Nachricht nach einem Tag erneut für einen Scan ein. Die Chancen sind groß, dass die Bewertung sich verändern könnte, wenn die Nachricht erneut eingereicht wird.

In der Zwischenzeit können Sie bösartige E-Mails aus den Posteingängen von Benutzern entfernen, indem Sie den Anleitungen in [diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) folgen.

- Kunden mit Microsoft Defender für Office 365 können:
    - den [Sicherheitsrisiken-Explorer zum Auffinden und Löschen von verdächtigen E-Mails](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered) verwenden
    - [Sichere Links zum Sperren von Zugriff](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) auf eine bösartige URL verwenden
    - Benutzer nachverfolgen, die auf bösartige URLs geklickt und zugegriffen haben: [Phishing-URL anzeigen und auf Bewertungsdaten klicken](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace).
    - manuell [eine automatische Untersuchung starten](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Sie können sich auch vor bösartigen Dateien und URLs, indem Sie die Anleitungen in [Schutz vor bösartigen URLs und Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) befolgen.