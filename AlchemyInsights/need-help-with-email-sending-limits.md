---
title: Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836278"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="60f2d-102">Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?</span><span class="sxs-lookup"><span data-stu-id="60f2d-102">Need help with email sending limits?</span></span>

<span data-ttu-id="60f2d-103">Unten finden Sie die im Dienst erzwungenen **entwurfsbedingte Sendegrenzen**.</span><span class="sxs-lookup"><span data-stu-id="60f2d-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="60f2d-104">Weitere Informationen zu diesen Grenzwerten sind [hier](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits) dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="60f2d-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="60f2d-105">Um von der Zustellung unerwünschter Massennachrichten abzuschrecken, wenden wir auf **alle ausgehenden und internen Nachrichten Grenzwerte für die Empfängerrate** pro Benutzer an.</span><span class="sxs-lookup"><span data-stu-id="60f2d-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="60f2d-106">In allen SKUs beträgt diese Grenze **10 000 Empfänger pro Tag**.</span><span class="sxs-lookup"><span data-stu-id="60f2d-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="60f2d-107">Kunden, die seriöse kommerzielle E-Mails versenden müssen (z. B. Kunden-Newsletter), sollten einen Drittanbieter in Anspruch nehmen, der sich auf diese Dienste spezialisiert.</span><span class="sxs-lookup"><span data-stu-id="60f2d-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="60f2d-108">**Hinweis**: Sobald die Empfängerratengrenze erreicht ist, können Nachrichten erst wieder aus dem Postfach gesendet werden, wenn die Anzahl von Empfängern, an die in den letzten 24 Stunden Nachrichten gesendet wurden, unter den Grenzwert fällt.</span><span class="sxs-lookup"><span data-stu-id="60f2d-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="60f2d-109">Der Benutzer kann bis zu diesem Zeitpunkt keine Nachrichten mehr senden.</span><span class="sxs-lookup"><span data-stu-id="60f2d-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="60f2d-110">Die Grenze der Nachrichtenrate von **30 Nachrichten pro Minute** gilt für alle SKUs.</span><span class="sxs-lookup"><span data-stu-id="60f2d-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="60f2d-111">Dadurch wird festgelegt, wie viele Nachrichten ein Benutzer innerhalb eines bestimmten Zeitraums von seinem Exchange Online-Konto aus senden kann.</span><span class="sxs-lookup"><span data-stu-id="60f2d-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="60f2d-112">Die **maximal zulässige Anzahl von Empfängern, die in den Feldern „An:“, „Cc:“ und „Bcc:“** für eine einzelne E-Mail-Nachricht über alle SKUs hinweg zulässig ist, beträgt **1000 Empfänger**.</span><span class="sxs-lookup"><span data-stu-id="60f2d-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="60f2d-113">Um diese Grenze anzupassen, gehen Sie [hier](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="60f2d-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
