---
title: Rückruf oder Ersetzen einer e-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: d5952041f6f2fd736e975abf06cc22880d21a089
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553431"
---
# <a name="recall-or-replace-an-email-message-in-office-365"></a>Rückruf oder Ersetzen einer e-Mail-Nachricht in Office 365

- Sie können **nur Nachrichten abrufen, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine gmail-Adresse gesendet wurde, können Sie Sie nicht mehr abrufen.
- Sie können **nur Nachrichten abrufen, die von Outlook 2016 für den PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Internet sendet, kann er nicht mehr daran erinnert werden.
- Wenn Sie Administrator sind, können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell abrufen**. Sie können keine Nachrichten aus dem Admin Center abrufen. Scrollen Sie nach unten zu "suchen und Löschen von e-Mail-Nachrichten in Ihrer Organisation", um weitere Informationen zu erhalten.

**Zurückrufen oder Ersetzen einer von Ihnen gesendeten e-Mail-Nachricht**

1. Wählen Sie im Bereich Ordner auf der linken Seite des Outlook-Fensters den Ordner Gesendete Elemente aus.
2. Öffnen Sie die Nachricht, die Sie abrufen möchten. Sie müssen doppelklicken, um die Nachricht zu öffnen. Wenn Sie die Nachricht auswählen, damit Sie im Lesebereich angezeigt wird, können Sie die Nachricht nicht mehr abrufen.
3. Wählen Sie auf der Registerkarte Nachricht die Option **Aktionen** > **Rückruf dieser Nachricht**aus.
4. Wählen Sie ungelesene **Kopien dieser Nachricht löschen** oder ungelesene **Kopien löschen aus, und ersetzen Sie Sie durch eine neue Nachricht, und**wählen Sie dann **OK**aus.
5. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **senden**aus.
6. Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen der Empfänger in Outlook ab.

Weitere Informationen, einschließlich der Vorgehensweise zum Überprüfen des Rückrufs, finden Sie unter [Rückruf oder Ersetzen einer von Ihnen gesendeten e-Mail-Nachricht](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Suchen nach und Löschen von e-Mail-Nachrichten in Ihrer Organisation*** Zum Suchen nach und Löschen von e-Mail-Nachrichten in Ihrer Organisation ist es am einfachsten, wenn Sie ein globaler Administrator sind. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rollengruppe "eDiscovery-Manager" oder der Rolle "Compliance Search Management" hinzugefügt werden. Wenn Sie Nachrichten löschen möchten, müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Rolle "Such-und Lösch Verwaltung" beitreten. Berechtigungen für diese Rollen werden im [Security #a0 Compliance Center](https://protection.office.com/)zugewiesen.

1. [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/office365/securitycompliance/content-search) , um die zu löschende Nachricht zu suchen.
2. Stellen [Sie eine Verbindung mit Security #a0 Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Wenn Sie MFA verwenden, finden Sie unter [Connect to Office 365 Security #a0 Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
