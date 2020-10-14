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
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451382"
---
# <a name="sendas-mail-enabled-public-folder"></a>E-Mail-aktivierter Öffentlicher Ordner für Absender

Im folgenden Beispiel wird dem Benutzer Jason die Berechtigung "Senden als" für den e-Mail-aktivierten Öffentlichen Ordner NewPF1 zugewiesen.

Add-RecipientPermission-Identity ' NewPF1 ' – Trustee "Jason" – AccessRights ' Sends '

Ausführliche Informationen zu Syntax und Parametern finden Sie unter Zuweisen von " [Senden als"-oder "Senden im Auftrag von"-Berechtigungen für e-Mail-aktivierte Öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

