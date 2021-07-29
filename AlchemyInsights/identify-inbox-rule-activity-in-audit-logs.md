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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630176"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen

Sie können die Überwachungsprotokollsuche im Microsoft 365 Security & Compliance Center verwenden, um Posteingangsregelereignisse anzuzeigen (Erstellen, Ändern und Löschen von Posteingangsregeln).

1. Melden Sie sich beim [Microsoft 365 Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur Suchseite des  >  **Überwachungsprotokolls** für die Suche.

3. Wählen Sie den Datumsbereich in den Feldern **Startdatum** und Enddatum aus. 

4. Überprüfen Sie unter **Exchange Postfachaktivitäten,** ob das Feld **"Aktivitäten"** auf **"Neue Posteingangsregel erstellen/ändern/aktivieren/deaktivieren"** festgelegt ist.

5. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Klicken Sie im Flyout "Details" auf **"Weitere Informationen".** Informationen zu den Posteingangsregeleinstellungen werden im **Parameterfeld** angezeigt.

Weitere Informationen finden Sie unter [Ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat.](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
