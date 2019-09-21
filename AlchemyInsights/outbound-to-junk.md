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
# <a name="outbound-email-to-junk-email-folder"></a>Ausgehende e-Mails in Junk-e-Mail-Ordner

Wenn Sie sehen, dass ausgehende Nachrichten als Junk markiert werden, führen Sie die folgenden Schritte aus:

- Wenn Sie dies noch nicht getan haben, sollten Sie die [Benachrichtigungen für ausgehende Spam Richtlinien konfigurieren](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).

- Verwenden Sie die [Nachrichtenablaufverfolgung](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) , um zu überprüfen, ob die ausgehende Nachricht den Ereignis Wert **Spam** mit dem zusätzlichen Detail: **use High Risk Delivery Pool**.

  Überprüfen Sie für diese Nachrichten den Nachrichteninhalt, um zu sehen, was als Spam eingestuft werden kann. Beispielsweise können Signaturen für viele Benutzer manchmal Probleme verursachen.

  Wenn Sie mehrere Beispiele für legitime ausgehende Nachrichten haben, die als Junk markiert sind, öffnen Sie ein Support Ticket, und bitten Sie den Support-Mitarbeiter, Ihre Nachrichten als falsch positive Ergebnisse an unsere Spam Analysten zu senden. Bereitstellen von Beispiel Nachrichten, die alle Nachrichtenkopfzeilen enthalten
