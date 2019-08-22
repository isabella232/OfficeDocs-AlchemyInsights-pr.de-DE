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
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539166"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen

Sie können die Überwachungsprotokoll Suche im Office 365 Security #a0 Compliance Center verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).

1. Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur **** > Suchseite**Überwachungsprotokoll** suchen.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. ****

4. Stellen Sie sicher, dass unter **Exchange-Postfachaktivitäten**das Feld **Aktivitäten** auf **neu-InboxRule Create/Modify/Enable/Disable Posteingangsregel**festgelegt ist.

5. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungseintrag aus. Klicken Sie im Detail Flyout auf **Weitere Informationen**. Im Feld **Parameter** werden Informationen zu den Einstellungen für Posteingangsregeln angezeigt.

Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) hat.
