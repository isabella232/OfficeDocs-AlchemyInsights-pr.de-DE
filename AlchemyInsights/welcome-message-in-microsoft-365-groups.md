---
title: Begrüßungsnachricht in Microsoft 365-Gruppen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725838"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="938a2-102">Begrüßungsnachricht in Microsoft 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="938a2-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="938a2-103">Neue Benutzer, die einer Microsoft 365-Gruppe beitreten, erhalten eine Begrüßungs-E-Mail, wenn die Eigenschaft „UnifiedGroupWelcomeMessageEnabled“ auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="938a2-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="938a2-104">Für den Fall, dass Sie die Begrüßungsnachricht deaktivieren möchten, verwenden Sie folgenden [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)-Befehl:</span><span class="sxs-lookup"><span data-stu-id="938a2-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
