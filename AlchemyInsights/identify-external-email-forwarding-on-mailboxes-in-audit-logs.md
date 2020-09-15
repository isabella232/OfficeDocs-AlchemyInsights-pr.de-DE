---
title: Identifizieren der externen e-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696296"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ermitteln, wann externe e-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Microsoft 365-Benutzer die externe e-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität im Rahmen des Cmdlets "Set **-Mailbox** " überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokoll Suche im Security & Compliance Center anzeigen.

1. Melden Sie sich beim [Microsoft 365 Security & Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur **Search**  >  Suchseite**Überwachungsprotokoll** suchen.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und **Enddatum** aus. Sie müssen keinen Benutzernamen angeben. Stellen Sie sicher, dass das Feld **Aktivitäten** auf **Ergebnisse für alle Aktivitäten anzeigen**festgelegt ist.

4. Klicken Sie auf **Suchen**.

Klicken Sie in den Ergebnissen auf **Filterergebnisse** , und geben Sie im Feld Aktivitäts Filter den Text **Satz-Postfach** ein. Wählen Sie einen Überwachungseintrag in den Ergebnissen aus. Klicken Sie im **Detail** Flyout auf **Weitere Informationen**. Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der e-Mail-Weiterleitung zusammenhängt.

- **ObjectID**: der Alias Wert des Postfachs, das geändert wurde.

- **Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-e-Mail-Adresse an.

- **UserID**: der Benutzer, der die e-Mail-Weiterleitung für das Postfach im Feld **objectID** konfiguriert hat.

Weitere Informationen finden Sie unter [bestimmen der Personen, die die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)haben.
