---
title: Konvertieren des Benutzerpostfachs in ein freigegebenes Postfach
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374322"
---
Sie können ein Benutzerpostfach nur in ein freigegebenes Postfach konvertieren, wenn der Benutzer über eine Exchange-Lizenz verfügt. Nachdem das Postfach konvertiert wurde, wird es weiterhin in der Liste der aktiven Benutzer angezeigt, da diese Liste freigegebene Postfächer enthält. Das konvertierte Postfach wird jedoch auch in der Liste freigegebener Postfächer angezeigt. 
  
Wenn Sie versuchen, ein Postfach in der Exchange-Verwaltungskonsole zu konvertieren, und die Konvertierung fehlschlägt, löschen Sie den Browsercache und die Cookies, und versuchen Sie es erneut. Wenn es immer noch nicht funktioniert, versuchen Sie, das Postfach in der Exchange-Verwaltungsshell zu konvertieren, indem Sie den folgenden Befehl ausführen:
  
```
Set-Mailbox -Type Shared
```

Weitere Informationen zur Post Fach Konvertierung finden [Sie unter Konvertieren eines Benutzerpostfachs in ein freigegebenes Postfach](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
