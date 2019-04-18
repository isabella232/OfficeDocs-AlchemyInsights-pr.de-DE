---
title: Identifizieren von Posteingangsregel Aktivitäten in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909242"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren von Posteingangsregel Aktivitäten in Überwachungsprotokollen

Sie können die Überwachungsprotokoll Suche im Security & Compliance Center verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).

1. Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. ****

4. Überprüfen Sie unter **Exchange-Postfachaktivitäten**, ob das Feld **Aktivitäten** auf **New-InboxRule erstellen/ändern/aktivieren/deaktivieren**der Posteingangsregel festgelegt ist.

5. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Klicken Sie im Detail Flyout auf **Weitere Informationen**. Informationen zu den Einstellungen für die Posteingangsregel werden im Feld **Parameter** angezeigt.

Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .
