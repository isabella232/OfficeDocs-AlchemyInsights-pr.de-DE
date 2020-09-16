---
title: Wiederherstellen gelöschter Elemente mit einem Cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741302"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="0a580-102">Wiederherstellen gelöschter Elemente mit einem Cmdlet</span><span class="sxs-lookup"><span data-stu-id="0a580-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="0a580-103">Verwenden Sie das Cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps), um gelöschte Elemente in Postfächern anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="0a580-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="0a580-104">Nachdem Sie die gelöschten Elemente gefunden haben, verwenden Sie das Cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps), um diese wiederherzustellen.</span><span class="sxs-lookup"><span data-stu-id="0a580-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="0a580-105">Die vollständigen Details hierzu finden Sie unter [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0a580-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="0a580-106">Um dieses Cmdlet ausführen zu können, muss Ihnen die Rolle „Postfachimport/-export“ zugewiesen worden sein.</span><span class="sxs-lookup"><span data-stu-id="0a580-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="0a580-107">Weitere Informationen finden Sie unter [Get-](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0a580-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
