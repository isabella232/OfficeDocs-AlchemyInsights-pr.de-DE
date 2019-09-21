---
title: Ausgehende e-Mails in Junk-e-Mail-Ordner
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062776"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="578a7-102">Ausgehende e-Mails in Junk-e-Mail-Ordner</span><span class="sxs-lookup"><span data-stu-id="578a7-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="578a7-103">Wenn Sie sehen, dass ausgehende Nachrichten als Junk markiert werden, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="578a7-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="578a7-104">Wenn Sie dies noch nicht getan haben, sollten Sie die [Benachrichtigungen für ausgehende Spam Richtlinien konfigurieren](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="578a7-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="578a7-105">Verwenden Sie die [Nachrichtenablaufverfolgung](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) , um zu überprüfen, ob die ausgehende Nachricht den Ereignis Wert **Spam** mit dem zusätzlichen Detail: **use High Risk Delivery Pool**.</span><span class="sxs-lookup"><span data-stu-id="578a7-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="578a7-106">Überprüfen Sie für diese Nachrichten den Nachrichteninhalt, um zu sehen, was als Spam eingestuft werden kann.</span><span class="sxs-lookup"><span data-stu-id="578a7-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="578a7-107">Beispielsweise können Signaturen für viele Benutzer manchmal Probleme verursachen.</span><span class="sxs-lookup"><span data-stu-id="578a7-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="578a7-108">Wenn Sie mehrere Beispiele für legitime ausgehende Nachrichten haben, die als Junk markiert sind, öffnen Sie ein Support Ticket, und bitten Sie den Support-Mitarbeiter, Ihre Nachrichten als falsch positive Ergebnisse an unsere Spam Analysten zu senden.</span><span class="sxs-lookup"><span data-stu-id="578a7-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="578a7-109">Bereitstellen von Beispiel Nachrichten, die alle Nachrichtenkopfzeilen enthalten</span><span class="sxs-lookup"><span data-stu-id="578a7-109">Be prepared to provide sample messages that include all message headers.</span></span>
