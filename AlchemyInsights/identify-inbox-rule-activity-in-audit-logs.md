---
title: Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383024"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen

Sie können die Überwachungsprotokoll Suche im Security #a0 Compliance Center verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).

1. Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. ****

4. Stellen Sie sicher, dass unter **Exchange-Postfachaktivitäten**das Feld **Aktivitäten** auf **neu-InboxRule Create/Modify/Enable/Disable Posteingangsregel**festgelegt ist.

5. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungseintrag aus. Klicken Sie im Detail Flyout auf **Weitere Informationen**. Im Feld **Parameter** werden Informationen zu den Einstellungen für Posteingangsregeln angezeigt.

Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) hat.
