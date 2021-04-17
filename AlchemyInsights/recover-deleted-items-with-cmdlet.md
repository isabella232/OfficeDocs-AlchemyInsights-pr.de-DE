---
title: Wiederherstellen gelöschter Elemente mit einem Cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835810"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="8e931-102">Wiederherstellen gelöschter Elemente mit einem Cmdlet</span><span class="sxs-lookup"><span data-stu-id="8e931-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="8e931-103">Verwenden Sie das Cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps), um gelöschte Elemente in Postfächern anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="8e931-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="8e931-104">Nachdem Sie die gelöschten Elemente gefunden haben, verwenden Sie das Cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps), um diese wiederherzustellen.</span><span class="sxs-lookup"><span data-stu-id="8e931-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="8e931-105">Die vollständigen Details hierzu finden Sie unter [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="8e931-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="8e931-106">Um dieses Cmdlet ausführen zu können, muss Ihnen die Rolle „Postfachimport/-export“ zugewiesen worden sein.</span><span class="sxs-lookup"><span data-stu-id="8e931-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="8e931-107">Weitere Informationen finden Sie unter [Get-](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="8e931-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
