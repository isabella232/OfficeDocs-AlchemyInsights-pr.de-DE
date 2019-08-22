---
title: Konvertieren eines Benutzerpostfachs in ein freigegebenes Postfach
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496398"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Konvertieren eines Benutzer-e-Mail-Felds in ein freigegebenes Postfach

Sie können ein Benutzerpostfach nur dann in ein freigegebenes Postfach konvertieren, wenn der Benutzer über eine Exchange-Lizenz verfügt. Nachdem das Postfach konvertiert wurde, wird es weiterhin in der Liste der aktiven Benutzer angezeigt, da diese Liste freigegebene Postfächer enthält. Das konvertierte Postfach wird jedoch auch in der Liste freigegebene Postfächer angezeigt. 
  
Wenn Sie versuchen, ein Postfach in der Exchange-Verwaltungskonsole zu konvertieren, und die Konvertierung fehlschlägt, löschen Sie den Browsercache und die Cookies, und versuchen Sie es erneut. Wenn es immer noch nicht funktioniert, versuchen Sie, das Postfach in der Exchange-Verwaltungsshell zu konvertieren, indem Sie den folgenden Befehl ausführen:
  
```
Set-Mailbox -Type Shared
```

Weitere Informationen zur Post Fach Konvertierung finden [Sie unter Konvertieren eines Benutzerpostfachs in ein freigegebenes Postfach](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
