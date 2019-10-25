---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682136"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen mit der Zustellung von e-Mails bei Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einem öffentlich verfügbaren SPF-oder DNS-Eintrags Prüfer im Internet.

Stellen Sie sicher, dass die ausgehende Nachricht von Office 365 nicht als Spam identifiziert und über den [Pool mit hoher Risikoverteilung](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)weitergeleitet wurde. Nachrichten im Pool mit hoher Risikoverteilung werden keine SPF-Prüfungen übergeben und werden daher von der Ziel-e-Mail-Organisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des e-Mail-Hosts wenden, an den Sie e-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Bounce-Nachricht verfügbar ist.  Office 365 Support kann möglicherweise nicht weiterhelfen.