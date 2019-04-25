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
<span data-ttu-id="9a089-102">Sie können ein Benutzerpostfach nur in ein freigegebenes Postfach konvertieren, wenn der Benutzer über eine Exchange-Lizenz verfügt.</span><span class="sxs-lookup"><span data-stu-id="9a089-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="9a089-103">Nachdem das Postfach konvertiert wurde, wird es weiterhin in der Liste der aktiven Benutzer angezeigt, da diese Liste freigegebene Postfächer enthält.</span><span class="sxs-lookup"><span data-stu-id="9a089-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="9a089-104">Das konvertierte Postfach wird jedoch auch in der Liste freigegebener Postfächer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9a089-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="9a089-105">Wenn Sie versuchen, ein Postfach in der Exchange-Verwaltungskonsole zu konvertieren, und die Konvertierung fehlschlägt, löschen Sie den Browsercache und die Cookies, und versuchen Sie es erneut.</span><span class="sxs-lookup"><span data-stu-id="9a089-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="9a089-106">Wenn es immer noch nicht funktioniert, versuchen Sie, das Postfach in der Exchange-Verwaltungsshell zu konvertieren, indem Sie den folgenden Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="9a089-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="9a089-107">Weitere Informationen zur Post Fach Konvertierung finden [Sie unter Konvertieren eines Benutzerpostfachs in ein freigegebenes Postfach](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="9a089-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
