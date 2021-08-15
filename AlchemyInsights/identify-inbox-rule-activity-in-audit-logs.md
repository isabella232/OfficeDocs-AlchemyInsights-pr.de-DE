---
title: Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976864"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen

Sie können die Überwachungsprotokollsuche im Microsoft 365 Security & Compliance Center verwenden, um Posteingangsregelereignisse anzuzeigen (Erstellen, Ändern und Löschen von Posteingangsregeln).

1. Melden Sie sich beim [Microsoft 365 Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur Suchseite des  >  **Überwachungsprotokolls** für die Suche.

3. Wählen Sie den Datumsbereich in den Feldern **Startdatum** und Enddatum aus. 

4. Überprüfen Sie unter **Exchange Postfachaktivitäten,** ob das Feld **"Aktivitäten"** auf **"New-InboxRule Create/modify/enable/disable"-Posteingangsregel** festgelegt ist.

5. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Klicken Sie im Flyout "Details" auf **"Weitere Informationen".** Informationen zu den Posteingangsregeleinstellungen werden im **Parameterfeld** angezeigt.

Weitere Informationen finden Sie unter [Ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat.](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
