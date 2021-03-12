---
title: Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736687"
---
# <a name="fix-tenant-policy-action-override"></a>Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)

Eine Antispamrichtlinie in Ihrem Mandanten hat diese Nachricht beeinflusst. Gehen Sie wie folgt vor, um die Richtlinie zu überprüfen:

1. Wechseln Sie zum [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)und wechseln Sie dann zu **Bedrohungsverwaltungsrichtlinie**  >    >  [Antispam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Überprüfen Sie, ob **die Richtlinienquelle** Folgendes angibt:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Wenn ja, überprüfen **Sie** auf der Registerkarte Benutzerdefinierte Die Einstellungen der Richtlinie, die sich auf die Nachricht ausdingt. Es ist möglich, dass die **Standardeinstellungen, die** auf alle Exchange Online Protection-Kunden angewendet wurden, die Nachricht beeinflusst haben.

Weitere Informationen zum Konfigurieren von Spamfilterrichtlinien finden Sie unter [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).
