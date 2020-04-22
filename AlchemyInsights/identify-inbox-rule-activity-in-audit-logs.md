---
title: Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716423"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen

Sie können die Überwachungsprotokoll Suche im Compliance Center von Microsoft 365 Security & verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).

1. Melden Sie sich beim [Microsoft 365 Security & Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur **Search** > Suchseite**Überwachungsprotokoll** suchen.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und **Enddatum** aus.

4. Stellen Sie sicher, dass unter **Exchange-Postfachaktivitäten**das Feld **Aktivitäten** auf **neu-InboxRule Create/Modify/Enable/Disable Posteingangsregel**festgelegt ist.

5. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungseintrag aus. Klicken Sie im Detail Flyout auf **Weitere Informationen**. Im Feld **Parameter** werden Informationen zu den Einstellungen für Posteingangsregeln angezeigt.

Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) hat.
