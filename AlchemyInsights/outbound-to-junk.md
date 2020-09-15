---
title: Ausgehende e-Mails in Junk-e-Mail-Ordner
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
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769182"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="f7134-102">Ausgehende e-Mails in Junk-e-Mail-Ordner</span><span class="sxs-lookup"><span data-stu-id="f7134-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="f7134-103">Wenn Sie sehen, dass ausgehende Nachrichten als Junk markiert werden, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="f7134-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="f7134-104">Wenn Sie dies noch nicht getan haben, sollten Sie die [Benachrichtigungen für ausgehende Spam Richtlinien konfigurieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="f7134-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="f7134-105">Verwenden Sie die [Nachrichtenablaufverfolgung](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) , um zu überprüfen, ob die ausgehende Nachricht den Ereignis Wert **Spam** mit dem zusätzlichen Detail: **use High Risk Delivery Pool**.</span><span class="sxs-lookup"><span data-stu-id="f7134-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="f7134-106">Überprüfen Sie für diese Nachrichten den Nachrichteninhalt, um zu sehen, was als Spam eingestuft werden kann.</span><span class="sxs-lookup"><span data-stu-id="f7134-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="f7134-107">Beispielsweise können Signaturen für viele Benutzer manchmal Probleme verursachen.</span><span class="sxs-lookup"><span data-stu-id="f7134-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="f7134-108">Wenn Sie mehrere Beispiele für legitime ausgehende Nachrichten haben, die als Junk markiert sind, öffnen Sie ein Support Ticket, und bitten Sie den Support-Mitarbeiter, Ihre Nachrichten als falsch positive Ergebnisse an unsere Spam Analysten zu senden.</span><span class="sxs-lookup"><span data-stu-id="f7134-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="f7134-109">Bereitstellen von Beispiel Nachrichten, die alle Nachrichtenkopfzeilen enthalten</span><span class="sxs-lookup"><span data-stu-id="f7134-109">Be prepared to provide sample messages that include all message headers.</span></span>
