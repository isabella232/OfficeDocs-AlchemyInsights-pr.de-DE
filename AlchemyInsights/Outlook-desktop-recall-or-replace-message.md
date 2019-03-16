---
title: Outlook-Desktop-Rückruf oder Ersetzen einer e-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657043"
---
# <a name="recall-or-replace-an-email-message"></a>Abrufen oder Ersetzen einer e-Mail-Nachricht

- Als Administrator können Sie **Nachrichten im Namen von Benutzern abrufen, die PowerShell verwenden**. Sie können keine Nachrichten aus dem Admin Center abrufen.
- Sie können **nur Nachrichten zurückrufen, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine gmail-Adresse gesendet wurde, können Sie Sie nicht mehr daran erinnern.
- Sie können **nur Nachrichten zurückrufen, die von Outlook 2016 auf dem PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Web sendet, können Sie ihn nicht mehr daran erinnern.

So können Sie eine e-Mail-Nachricht abrufen oder ersetzen:

1. Wählen Sie im Ordnerbereich auf der linken Seite des Outlook-Fensters den Ordner Gesendete Elemente aus.
1. Doppelklicken Sie auf die Nachricht, die Sie abrufen möchten, um Sie zu öffnen.
1. Wählen Sie die Registerkarte **Nachricht** aus, und wählen Sie dann **Aktionen** > **Diese Nachricht abrufen**aus.
1. Wählen Sie ungelesene **Kopien dieser Nachricht löschen** oder ungelesene **Kopien löschen und durch eine neue Nachricht ersetzen**, und klicken Sie dann auf **OK**.
1. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **senden**aus.
1. Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen des Empfängers in Outlook ab. Schritte zum Überprüfen des Rückrufs finden Sie in [diesem Artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Suchen und Löschen von e-Mail-Nachrichten in Ihrer Organisation

- Wenn Sie kein globaler Administrator sind, muss Ihr Konto der eDiscovery-Manager-Rolle oder der Compliance-Such Verwaltungsrolle hinzugefügt werden, um nach Nachrichten suchen zu können. Zum Löschen von Nachrichten müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Verwaltungsrolle "suchen und löschen" beitreten. Berechtigungen für diese Rollen werden im [Security and Compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731)zugewiesen.
- [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/office365/securitycompliance/content-search) , um die zu löschende Nachricht zu suchen.
- [Herstellen einer Verbindung mit der Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Wenn Sie mehrstufige Authentifizierung verwenden, finden Sie weitere Informationen unter [Connect to Office 365 Security and Compliance Center PowerShell using Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).