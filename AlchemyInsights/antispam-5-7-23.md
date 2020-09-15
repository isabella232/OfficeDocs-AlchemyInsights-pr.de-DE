---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717324"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen mit der Zustellung von e-Mails bei Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einem öffentlich verfügbaren SPF-oder DNS-Eintrags Prüfer im Internet.

Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den [Pool mit hoher Risikoverteilung](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)weitergeleitet wurde. Nachrichten im Pool mit hoher Risikoverteilung werden keine SPF-Prüfungen übergeben und werden daher von der Ziel-e-Mail-Organisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des e-Mail-Hosts wenden, an den Sie e-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Bounce-Nachricht verfügbar ist. Der Microsoft-Support kann möglicherweise nicht weiterhelfen.
