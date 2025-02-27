---
title: Durchsetzung des Postfach-Empfangslimit
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829162"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Durchsetzung des Postfach-Empfangslimit

Microsoft vor kurzem damit begonnen, den Schwellenwert von 3600 Nachrichten pro Stunde pro Postfach durchzusetzen. Weitere Informationen finden Sie unter [Exchange Online-Begrenzungen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 Postfächer, die innerhalb einer Stunde mehr als 3600 Nachrichten empfangen, werden für die nächsten 60 Minuten gedrosselt. 

Darüber hinaus wird der Grenzwert für Absender-Empfänger-Paare (AEP) angewendet, der Nachrichten blockiert, die ein Microsoft 365-Postfach von einem bestimmten Absender empfängt.  Wenn ein einzelner Absender mehr als 33 % des Gesamtschwellenwerts oder 1200 Nachrichten pro fortlaufender Stunde an einen bestimmten Empfänger sendet, tritt das AEP-Limit in Kraft, und das Postfach akzeptiert von diesem Absender keine weiteren Nachrichten mehr. Hinweis:

- Dieses Limit gilt für E-Mails, die von anderen Mandanten, lokalen oder Internet-Absendern empfangen werden.
- Die E-Mail-Zustellung an das Postfach wird ist die nächsten 60 Minuten blockiert. 
- Absender an diese Postfächer erhalten einen Unzustellbarkeitsbericht (5.2.121 oder 5.2.122), der angibt, dass das Postfach den maximalen Zustellungsschwellenwert überschritten hat. Interne Mandanten Nachrichten(E-Mails innerhalb desselben Mandanten) werden weiterhin zugestellt.
- Wenn der AEP-Grenzwert angewendet wird, nimmt das empfangende Postfach weiterhin Nachrichten von anderen Absendern an.

Administratoren können die aktuelle Postfachaktivität überwachen, indem sie auf einen neuen Bericht und Einblick in das Exchange Admin Center namens „Postfächer die die Empfangsgrenzen überschreiten“ zugreifen. Der Einblick wird nur angezeigt, wenn ein Mandant anstößige Postfächer hat, während der Bericht immer im Dashboard angezeigt wird, aber leer ist, es sei denn, ein Mandant hat ein anstößiges Postfach.

Weitere Informationen über den Einblick auf überschrittene Empfangslimits, finden Sie unter [Einblicke, im neuen EAC, auf Postfächer die die Empfangslimits überschritten haben](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Weitere Informationen zum Bericht über die Überschreitung von Empfangsgrenzwerten finden Sie unter [Bericht „Postfächer, die Empfangslimits überschreiten“ im neuen EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).