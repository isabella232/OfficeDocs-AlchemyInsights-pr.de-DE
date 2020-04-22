---
title: Ausgehende e-Mails in Junk-e-Mail-Ordner
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761167"
---
# <a name="outbound-email-to-junk-email-folder"></a>Ausgehende e-Mails in Junk-e-Mail-Ordner

Wenn Sie sehen, dass ausgehende Nachrichten als Junk markiert werden, führen Sie die folgenden Schritte aus:

- Wenn Sie dies noch nicht getan haben, sollten Sie die [Benachrichtigungen für ausgehende Spam Richtlinien konfigurieren](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).

- Verwenden Sie die [Nachrichtenablaufverfolgung](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) , um zu überprüfen, ob die ausgehende Nachricht den Ereignis Wert **Spam** mit dem zusätzlichen Detail: **use High Risk Delivery Pool**.

  Überprüfen Sie für diese Nachrichten den Nachrichteninhalt, um zu sehen, was als Spam eingestuft werden kann. Beispielsweise können Signaturen für viele Benutzer manchmal Probleme verursachen.

  Wenn Sie mehrere Beispiele für legitime ausgehende Nachrichten haben, die als Junk markiert sind, öffnen Sie ein Support Ticket, und bitten Sie den Support-Mitarbeiter, Ihre Nachrichten als falsch positive Ergebnisse an unsere Spam Analysten zu senden. Bereitstellen von Beispiel Nachrichten, die alle Nachrichtenkopfzeilen enthalten
