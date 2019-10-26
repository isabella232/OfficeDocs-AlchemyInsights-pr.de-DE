---
title: Fehlercode 550 5.7.501 Zugriff verweigert, Spam Missbrauch erkannt
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36740140"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501-Zugriff verweigert, Spam Missbrauch erkannt

Diese Meldung tritt normalerweise auf, wenn Benutzer e-Mail-Nachrichten von IP-Adressen mithilfe der Initial *. onmicrosoft.com* -Domäne senden, die neuen Mandanten in Office 365 zugewiesen ist. Am einfachsten lässt sich dieses Problem beheben:

1. [Hinzufügen einer Domäne zu Ihrem Mandanten](https://docs.microsoft.com//office365/admin/setup/add-domain).

2. [Ändern Sie die primäre e-Mail-Adresse Ihrer Benutzer](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) in die neue benutzerdefinierte Domäne, die Sie soeben hinzugefügt haben.
