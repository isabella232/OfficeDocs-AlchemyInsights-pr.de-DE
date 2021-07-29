---
title: Identifizieren der externen E-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630248"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ermitteln, wann die externe E-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Microsoft 365 Benutzer die externe E-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des Cmdlets **"Set-Mailbox"** überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokollsuche im Security & Compliance Center anzeigen.

1. Melden Sie sich beim [Microsoft 365 Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur Suchseite des  >  **Überwachungsprotokolls** für die Suche.

3. Wählen Sie den Datumsbereich in den Feldern **Startdatum** und Enddatum aus.  Sie müssen keinen Benutzernamen angeben. Überprüfen Sie, ob das Feld **"Aktivitäten"** auf **"Ergebnisse für alle Aktivitäten anzeigen"** festgelegt ist.

4. Klicken Sie auf **Suchen**.

Klicken Sie in den Ergebnissen auf **"Ergebnisse filtern",** und geben **Sie "Set-Mailbox"** im Aktivitätsfilterfeld ein. Wählen Sie einen Überwachungsdatensatz in den Ergebnissen aus. Klicken Sie im **Flyout "Details"** auf **"Weitere Informationen".** Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt.

- **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.

- **Parameter:** _ForwardingSmtpAddress_ gibt die E-Mail-Zieladresse an.

- **UserId**: Der Benutzer, der die E-Mail-Weiterleitung für das Postfach im **Feld ObjectId** konfiguriert hat.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet hat.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
