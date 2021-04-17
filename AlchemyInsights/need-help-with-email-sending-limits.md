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
# <a name="need-help-with-email-sending-limits"></a>Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?

Unten finden Sie die im Dienst erzwungenen **entwurfsbedingte Sendegrenzen**. Weitere Informationen zu diesen Grenzwerten sind [hier](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits) dokumentiert.

- Um von der Zustellung unerwünschter Massennachrichten abzuschrecken, wenden wir auf **alle ausgehenden und internen Nachrichten Grenzwerte für die Empfängerrate** pro Benutzer an. In allen SKUs beträgt diese Grenze **10 000 Empfänger pro Tag**.  Kunden, die seriöse kommerzielle E-Mails versenden müssen (z. B. Kunden-Newsletter), sollten einen Drittanbieter in Anspruch nehmen, der sich auf diese Dienste spezialisiert.
    - **Hinweis**: Sobald die Empfängerratengrenze erreicht ist, können Nachrichten erst wieder aus dem Postfach gesendet werden, wenn die Anzahl von Empfängern, an die in den letzten 24 Stunden Nachrichten gesendet wurden, unter den Grenzwert fällt. Der Benutzer kann bis zu diesem Zeitpunkt keine Nachrichten mehr senden.
- Die Grenze der Nachrichtenrate von **30 Nachrichten pro Minute** gilt für alle SKUs. Dadurch wird festgelegt, wie viele Nachrichten ein Benutzer innerhalb eines bestimmten Zeitraums von seinem Exchange Online-Konto aus senden kann.
- Die **maximal zulässige Anzahl von Empfängern, die in den Feldern „An:“, „Cc:“ und „Bcc:“** für eine einzelne E-Mail-Nachricht über alle SKUs hinweg zulässig ist, beträgt **1000 Empfänger**. Um diese Grenze anzupassen, gehen Sie [hier](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
