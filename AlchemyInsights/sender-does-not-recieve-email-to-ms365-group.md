---
title: Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751314"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="c2a30-102">Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail</span><span class="sxs-lookup"><span data-stu-id="c2a30-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="c2a30-103">Der Absender einer E-Mail-Nachricht an eine Microsoft 365-Gruppe empfängt standardmäßig keine Kopie der Nachricht in seinem Posteingang, auch er ein Mitglied der Gruppe ist.</span><span class="sxs-lookup"><span data-stu-id="c2a30-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="c2a30-104">Mit diesem EXO PowerShell-Befehl können Sie dem Absender das Empfangen einer Kopie jeder E-Mail erlauben, die er an die Microsoft 365-Gruppe sendet:</span><span class="sxs-lookup"><span data-stu-id="c2a30-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="c2a30-105">So aktivieren Sie die Einstellung für alle Postfächer gleichzeitig:</span><span class="sxs-lookup"><span data-stu-id="c2a30-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="c2a30-106">**Hinweis** Änderungen an dieser Einstellung dauern bis zu einer Stunde, bis sie wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="c2a30-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>