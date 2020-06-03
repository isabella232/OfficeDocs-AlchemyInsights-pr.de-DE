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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506442"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen mit der Zustellung von e-Mails bei Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einem öffentlich verfügbaren SPF-oder DNS-Eintrags Prüfer im Internet.

Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den [Pool mit hoher Risikoverteilung](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)weitergeleitet wurde. Nachrichten im Pool mit hoher Risikoverteilung werden keine SPF-Prüfungen übergeben und werden daher von der Ziel-e-Mail-Organisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des e-Mail-Hosts wenden, an den Sie e-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Bounce-Nachricht verfügbar ist. Der Microsoft-Support kann möglicherweise nicht weiterhelfen.
