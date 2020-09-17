---
title: Fehlercode 550 5.7.501 Zugriff verweigert, Spam Missbrauch erkannt
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784054"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501-Zugriff verweigert, Spam Missbrauch erkannt

Diese Meldung tritt normalerweise auf, wenn Benutzer e-Mail-Nachrichten von IP-Adressen mithilfe der anfänglichen *. onmicrosoft.com* -Domäne senden, die neuen Mandanten in Microsoft 365 zugewiesen ist. Am einfachsten lässt sich dieses Problem beheben:

1. [Hinzufügen einer Domäne zu Ihrem Mandanten](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Ändern Sie die primäre e-Mail-Adresse Ihrer Benutzer](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) in die neue benutzerdefinierte Domäne, die Sie soeben hinzugefügt haben.
