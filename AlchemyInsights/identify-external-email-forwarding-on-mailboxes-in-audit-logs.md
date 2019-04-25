---
title: Identifizieren der externen e-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417211"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifizieren, wann externe e-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Benutzer die externe e-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des Cmdlets **Set-Mailbox** überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokoll Suche im Security & Compliance Center anzeigen.

1. Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. **** Sie müssen keinen Benutzernamen angeben. Stellen Sie sicher, dass das Feld **Aktivitäten** auf **Ergebnisse für alle Aktivitäten anzeigen**festgelegt ist.

4. Klicken Sie auf **Suchen**.

Klicken Sie in den Ergebnissen auf **Ergebnisse filtern** , und geben Sie **Set-Mailbox** in das Feld Aktivitäts Filter ein. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Klicken Sie im **Detail** Flyout auf **Weitere Informationen**. Sie müssen sich die Details der einzelnen Überwachungsdatensätze ansehen, um festzustellen, ob die Aktivität mit der e-Mail-Weiterleitung verbunden ist.

- **ObjectID**: der Alias Wert des Postfachs, das geändert wurde.

- **Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-e-Mail-Adresse an.

- **UserID**: der Benutzer, der die e-Mail-Weiterleitung für das Postfach im **objectID** -Feld konfiguriert hat.

Weitere Informationen finden Sie unter [bestimmen der Benutzer, die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)haben.
