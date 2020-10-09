---
title: Öffentlichen Ordner "als e-Mail-aktiviert senden" in Exo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394688"
---
# <a name="sendas-mail-enabled-public-folder"></a>E-Mail-aktivierter Öffentlicher Ordner für Absender

Im folgenden Beispiel wird dem Benutzer Jason die Berechtigung "Senden als" für den e-Mail-aktivierten Öffentlichen Ordner NewPF1 zugewiesen.

Add-RecipientPermission-Identity ' NewPF1 ' – Trustee "Jason" – AccessRights ' Sends '

Ausführliche Informationen zu Syntax und Parametern finden Sie unter Zuweisen von " [Senden als"-oder "Senden im Auftrag von"-Berechtigungen für e-Mail-aktivierte Öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).
