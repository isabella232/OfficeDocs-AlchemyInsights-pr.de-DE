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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034933"
---
# <a name="fix-tenant-policy-action-override"></a>Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)

Diese Nachricht wurde durch eine Antispamrichtlinie in Ihrem Mandanten beeinflusst. Gehen Sie folgendermaßen vor, um die Richtlinie zu überprüfen:

1. Wechseln Sie zum [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)und wechseln Sie dann zu   >    >  ["Antispamrichtlinie](https://go.microsoft.com/fwlink/?linkid=2101518)für die Bedrohungsverwaltung".
2. Überprüfen Sie, ob **die Richtlinienquelle** Folgendes angibt:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC message**

    Wenn ja, überprüfen Sie auf der Registerkarte **"Benutzerdefiniert"** die Einstellungen der Richtlinie, die die Nachricht beeinflusst hat. Es ist möglich, dass die **Standardeinstellungen,** die auf alle Exchange Online Protection Kunden angewendet wurden, die Nachricht betroffen haben.

Weitere Informationen zum Konfigurieren von Spamfilterrichtlinien finden Sie unter [Konfigurieren ihrer Spamfilterrichtlinien.](https://go.microsoft.com/fwlink/?linkid=2101431)
