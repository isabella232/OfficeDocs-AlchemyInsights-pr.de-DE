---
title: Mikroverzögerungen oder Drosselung in Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702125"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="a277c-102">Mikroverzögerungen oder Drosselung in Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a277c-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="a277c-103">Möglicherweise wird beim Ausführen von Skripts und Cmdlets in Exchange Online die Warnung "Mikroverzögerung angewendet" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a277c-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="a277c-104">Hier sind einige Vorschläge, wie Sie das Problem lösen können:</span><span class="sxs-lookup"><span data-stu-id="a277c-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="a277c-105">Bitte führen Sie unsere Diagnose aus, um die PowerShell-Drosselungsrichtlinien Ihres Mandanten zu entspannen.</span><span class="sxs-lookup"><span data-stu-id="a277c-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="a277c-106">Diese Lösung wird das Problem für die meisten Personen lösen.</span><span class="sxs-lookup"><span data-stu-id="a277c-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="a277c-107">Wenn das Problem noch nicht behoben ist, verwenden Sie das [Exchange Online v2 PowerShell-Modul](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), das Cmdlets enthält, die auf REST-API basieren und wesentlich performanter sind.</span><span class="sxs-lookup"><span data-stu-id="a277c-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="a277c-108">Dies kann eine großartige Lösung für viele Get-Cmdlets sein, die häufig verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="a277c-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="a277c-109">Wenn Sie CMDlets verwenden müssen, die nicht im v2-Modul abgedeckt sind, lesen Sie bitte [Ausführen von PowerShell-Cmdlets für eine große Anzahl von Benutzern in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), in dem beschrieben wird, wie Sie die PowerShell-Drosselungsgrenzen in Exchange Online umgehen können.</span><span class="sxs-lookup"><span data-stu-id="a277c-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
