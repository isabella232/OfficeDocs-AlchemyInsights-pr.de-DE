---
title: Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702362"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="2c4fb-102">Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?</span><span class="sxs-lookup"><span data-stu-id="2c4fb-102">Need help with email sending limits?</span></span>

<span data-ttu-id="2c4fb-103">Unten finden Sie die im Dienst erzwungenen **entwurfsbedingte Sendegrenzen**.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="2c4fb-104">Weitere Informationen zu diesen Grenzwerten sind [hier](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits) dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="2c4fb-105">Um von der Zustellung unerwünschter Massennachrichten abzuschrecken, wenden wir auf **alle ausgehenden und internen Nachrichten Grenzwerte für die Empfängerrate** pro Benutzer an.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="2c4fb-106">In allen SKUs beträgt diese Grenze **10 000 Empfänger pro Tag**.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="2c4fb-107">Kunden, die seriöse kommerzielle E-Mails versenden müssen (z. B. Kunden-Newsletter), sollten einen Drittanbieter in Anspruch nehmen, der sich auf diese Dienste spezialisiert.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="2c4fb-108">**Hinweis**: Sobald die Empfängerratengrenze erreicht ist, können Nachrichten erst wieder aus dem Postfach gesendet werden, wenn die Anzahl von Empfängern, an die in den letzten 24 Stunden Nachrichten gesendet wurden, unter den Grenzwert fällt.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="2c4fb-109">Der Benutzer kann bis zu diesem Zeitpunkt keine Nachrichten mehr senden.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="2c4fb-110">Die Grenze der Nachrichtenrate von **30 Nachrichten pro Minute** gilt für alle SKUs.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="2c4fb-111">Dadurch wird festgelegt, wie viele Nachrichten ein Benutzer innerhalb eines bestimmten Zeitraums von seinem Exchange Online-Konto aus senden kann.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="2c4fb-112">Die **maximal zulässige Anzahl von Empfängern, die in den Feldern „An:“, „Cc:“ und „Bcc:“** für eine einzelne E-Mail-Nachricht über alle SKUs hinweg zulässig ist, beträgt **1000 Empfänger**.</span><span class="sxs-lookup"><span data-stu-id="2c4fb-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="2c4fb-113">Um diese Grenze anzupassen, gehen Sie [hier](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="2c4fb-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
