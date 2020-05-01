---
title: Mikroverzögerungen oder Drosselung in Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947830"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="2729b-102">Mikroverzögerungen oder Drosselung in Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="2729b-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="2729b-103">Möglicherweise wird beim Ausführen von Skripts und Cmdlets in Exchange Online die Warnung "Mikroverzögerung angewendet" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2729b-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="2729b-104">Hier sind zwei Vorschläge, die sich auf dieses Thema beziehen:</span><span class="sxs-lookup"><span data-stu-id="2729b-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="2729b-105">Sie können versuchen, das [Exchange Online v2 PowerShell-Modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) zu verwenden, das Cmdlets enthält, die auf REST-API basieren und wesentlich performanter sind.</span><span class="sxs-lookup"><span data-stu-id="2729b-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="2729b-106">Dies kann eine großartige Lösung für viele Get-Cmdlets sein, die häufig verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2729b-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="2729b-107">Wenn Sie Cmdlets verwenden müssen, die vom V2-Modul noch nicht abgedeckt sind, lesen Sie [Ausführen von PowerShell-Cmdlets für eine große Anzahl von Benutzern in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). In diesem Artikel wird erläutert, wie Sie die erwarteten PowerShell-Drosselungs-Limits in Exchange Online umgehen.</span><span class="sxs-lookup"><span data-stu-id="2729b-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
