---
title: Meldung „Keine Abonnements gefunden“ im Security Center
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768530"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Meldung „Keine Abonnements gefunden“ im Security Center

Wenn Sie beim Zugriff auf das Microsoft Defender Security Center die Meldung „Keine Abonnements gefunden“ erhalten, bedeutet dies, dass das Azure Active Directory (AAD), mit dem sich der Benutzer am Portal anmeldet, keine Microsoft Defender ATP-Lizenz hat.  

Die Lizenzen für Windows E5 und Office E5 sind separate Lizenzen.

Öffnen Sie einen Supportfall, wenn die Lizenz erworben, aber nicht für diese AAD-Instanz bereitgestellt wurde. Entweder tritt <br/>
-   ein mögliches Problem bei der Lizenzbereitstellung auf.<br/>
-   Oder Sie haben die Lizenz versehentlich für ein anderes Microsoft AAD als das für die Authentifizierung beim Dienst verwendete bereitgestellt.