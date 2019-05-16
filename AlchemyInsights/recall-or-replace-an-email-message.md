---
title: Abrufen oder Ersetzen einer e-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096502"
---
# <a name="recall-or-replace-an-email-message"></a>Abrufen oder Ersetzen einer e-Mail-Nachricht

- Sie können **nur Nachrichten zurückrufen, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine gmail-Adresse gesendet wurde, können Sie Sie nicht mehr daran erinnern.
- Sie können **nur Nachrichten zurückrufen, die von Outlook 2016 für den PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Web sendet, können Sie ihn nicht mehr daran erinnern.
- Wenn Sie ein Administrator sind, können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell abrufen**. Sie können keine Nachrichten aus dem Admin Center abrufen. Führen Sie einen Bildlauf nach unten durch, um nach e-Mail-Nachrichten in Ihrer Organisation zu suchen und diese zu löschen.

***Zurückrufen oder Ersetzen einer gesendeten e-Mail-Nachricht***
1. Klicken Sie im Ordnerbereich auf der linken Seite des Outlook-Fensters auf den Ordner "Gesendete Elemente".
2. Öffnen Sie die Nachricht, die Sie abrufen möchten. Sie müssen doppelklicken, um die Nachricht zu öffnen. Wenn Sie die Nachricht auswählen, sodass Sie im Lesebereich angezeigt wird, können Sie die Nachricht nicht mehr abrufen.
3. Wählen Sie auf der Registerkarte Nachricht die Option **Aktionen** > **Diese Nachricht abrufen**aus.
4. Wählen Sie ungelesene **Kopien dieser Nachricht löschen** oder ungelesene **Kopien löschen und durch eine neue Nachricht ersetzen, und**klicken Sie dann auf **OK**.
5. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **senden**aus.
6. Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen des Empfängers in Outlook ab. 

Weitere Informationen, einschließlich der Überprüfung des Rückrufs, finden Sie unter [Rückruf oder Ersetzen einer e-Mail-Nachricht, die Sie gesendet](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)haben.

***Suchen und Löschen von e-Mail-Nachrichten in Ihrer Organisation*** Zum Suchen und Löschen von e-Mail-Nachrichten in Ihrer Organisation ist es am einfachsten, wenn Sie ein globaler Administrator sind. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rollengruppe eDiscovery-Manager oder der Verwaltungsrolle Compliance Search hinzugefügt werden. Zum Löschen von Nachrichten müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Verwaltungsrolle "suchen und löschen" beitreten. Berechtigungen für diese Rollen werden im [Security & Compliance Center](https://protection.office.com/)zugewiesen.

1. [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) , um die zu löschende Nachricht zu suchen.
2. Stellen [Sie eine Verbindung mit Security & Compliance Center PowerShell her](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Wenn Sie MFA verwenden, finden Sie unter [Connect to Office 365 Security & Compliance Center PowerShell mithilfe der mehr](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)stufigen Authentifizierung. 