---
title: Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2020
ms.locfileid: "46846055"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail

Der Absender einer E-Mail-Nachricht an eine Microsoft 365-Gruppe empfängt standardmäßig keine Kopie der Nachricht in seinem Posteingang, auch er ein Mitglied der Gruppe ist.

Mit diesem EXO PowerShell-Befehl können Sie dem Absender das Empfangen einer Kopie jeder E-Mail erlauben, die er an die Microsoft 365-Gruppe sendet:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

So aktivieren Sie die Einstellung für alle Postfächer gleichzeitig:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Hinweis** Änderungen an dieser Einstellung dauern bis zu einer Stunde, bis sie wirksam werden.