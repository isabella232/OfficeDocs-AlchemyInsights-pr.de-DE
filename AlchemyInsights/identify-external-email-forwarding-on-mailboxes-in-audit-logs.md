---
title: Identifizieren der externen e-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383096"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ermitteln, wann externe e-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Benutzer die externe e-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität im Rahmen des Cmdlets "Set **-Mailbox** " überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokoll Suche im Security #a0 Compliance Center anzeigen.

1. Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. **** Sie müssen keinen Benutzernamen angeben. Stellen Sie sicher, dass das Feld **Aktivitäten** auf **Ergebnisse für alle Aktivitäten anzeigen**festgelegt ist.

4. Klicken Sie auf **Suchen**.

Klicken Sie in den Ergebnissen auf **Filterergebnisse** , und geben Sie im Feld Aktivitäts Filter den Text **Satz-Postfach** ein. Wählen Sie einen Überwachungseintrag in den Ergebnissen aus. Klicken Sie im **Detail** Flyout auf **Weitere Informationen**. Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der e-Mail-Weiterleitung zusammenhängt.

- **ObjectID**: der Alias Wert des Postfachs, das geändert wurde.

- **Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-e-Mail-Adresse an.

- **UserID**: der Benutzer, der die e-Mail-Weiterleitung für das Postfach im Feld **objectID** konfiguriert hat.

Weitere Informationen finden Sie unter [bestimmen der Personen, die die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)haben.
