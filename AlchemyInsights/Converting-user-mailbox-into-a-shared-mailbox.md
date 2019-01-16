---
title: Konvertieren von Postfach des Benutzers in einem freigegebenen Postfach?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290073"
---
<span data-ttu-id="5e3d7-p101">Sie können nur ein Benutzerpostfach auf ein freigegebenes Postfach konvertieren, wenn der Benutzer eine Exchange-Lizenz verfügt. Nachdem das Postfach konvertiert wurde, wird weiterhin in der Liste der aktiven Benutzer angezeigt wird, da diese Liste freigegebene Postfächer enthält. Allerdings werden die konvertierte Mailbox auch in der Liste freigegebenes Postfach angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5e3d7-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="5e3d7-p102">Wenn Sie versuchen, ein Postfach in der Exchange-Verwaltungskonsole zu konvertieren, und die Konvertierung ein Fehler auftritt, deaktivieren Sie Ihre Browsercaches und Cookies, und versuchen Sie es erneut. Wenn weiterhin nicht funktioniert, wiederholen Sie die Konvertierung von des Postfachs in der Exchange-Verwaltungsshell mithilfe des folgenden Befehls:</span><span class="sxs-lookup"><span data-stu-id="5e3d7-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="5e3d7-107">Weitere Informationen zur Konvertierung Postfach steht in [ein Benutzerpostfach auf ein freigegebenes Postfach zu konvertieren](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="5e3d7-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
