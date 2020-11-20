---
title: Rückruf oder Ersetzen einer e-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353505"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Rückruf oder Ersetzen einer e-Mail-Nachricht in Microsoft 365

- Sie können **nur Nachrichten abrufen, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine gmail-Adresse gesendet wurde, können Sie Sie nicht mehr abrufen.
- Sie können **nur Nachrichten abrufen, die von Outlook für den PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Internet sendet, kann er nicht mehr daran erinnert werden.
- Als mandantenadministrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell abrufen** (Weitere Informationen finden Sie unter: [Suchen nach und Löschen von e-Mail-Nachrichten](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Sie können keine Nachrichten aus dem Admin Center abrufen. Scrollen Sie nach unten zu "suchen und Löschen von e-Mail-Nachrichten in Ihrer Organisation", um weitere Informationen zu erhalten.

**Zurückrufen oder Ersetzen einer von Ihnen gesendeten e-Mail-Nachricht**

1. Wählen Sie im Bereich Ordner auf der linken Seite des Outlook-Fensters den Ordner Gesendete Elemente aus.
2. Öffnen Sie die Nachricht, die Sie abrufen möchten. Sie müssen doppelklicken, um die Nachricht zu öffnen. Wenn Sie die Nachricht auswählen, damit Sie im Lesebereich angezeigt wird, können Sie die Nachricht nicht mehr abrufen.
3. Wählen Sie auf der Registerkarte Nachricht die Option **Aktionen**  >  **Rückruf dieser Nachricht** aus.
4. Wählen Sie **Ungelesene Kopien dieser Nachricht löschen** oder **Ungelesene Kopien löschen aus, und ersetzen Sie Sie durch eine neue Nachricht, und** wählen Sie dann **OK** aus.
5. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **senden** aus.
6. Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen der Empfänger in Outlook ab.

Weitere Informationen, einschließlich der Vorgehensweise zum Überprüfen des Rückrufs, finden Sie unter [Rückruf oder Ersetzen einer von Ihnen gesendeten e-Mail-Nachricht](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Zum Suchen nach und Löschen von e-Mail-Nachrichten in Ihrer Organisation_** ist es am einfachsten, wenn Sie ein globaler Administrator sind. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rollengruppe "eDiscovery-Manager" oder der Rolle "Compliance Search Management" hinzugefügt werden. Wenn Sie Nachrichten löschen möchten, müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Rolle "Such-und Lösch Verwaltung" beitreten. Berechtigungen für diese Rollen werden im [Security & Compliance Center](https://protection.office.com/)zugewiesen.

1. [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu suchen.
2. [Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Wenn Sie MFA (Multi-Factor Authentication) verwenden, finden Sie unter [Connect to Microsoft 365 Security & Compliance Center PowerShell mit mehr](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)stufiger Authentifizierung.
