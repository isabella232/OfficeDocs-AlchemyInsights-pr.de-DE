---
title: Konvertieren von Postfach des Benutzers in einem freigegebenen Postfach?
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906731"
---
Sie können nur ein Benutzerpostfach auf ein freigegebenes Postfach konvertieren, wenn der Benutzer eine Exchange-Lizenz verfügt. Nachdem das Postfach konvertiert wurde, wird weiterhin in der Liste der aktiven Benutzer angezeigt wird, da diese Liste freigegebene Postfächer enthält. Allerdings werden die konvertierte Mailbox auch in der Liste freigegebenes Postfach angezeigt. 
  
Wenn Sie versuchen, ein Postfach in der Exchange-Verwaltungskonsole zu konvertieren, und die Konvertierung ein Fehler auftritt, deaktivieren Sie Ihre Browsercaches und Cookies, und versuchen Sie es erneut. Wenn weiterhin nicht funktioniert, wiederholen Sie die Konvertierung von des Postfachs in der Exchange-Verwaltungsshell mithilfe des folgenden Befehls:
  
```
Set-Mailbox -Type Shared
```

Weitere Informationen zur Konvertierung Postfach steht in [ein Benutzerpostfach auf ein freigegebenes Postfach zu konvertieren](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
