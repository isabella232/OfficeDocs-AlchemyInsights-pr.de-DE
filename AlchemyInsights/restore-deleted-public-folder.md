---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809438"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="3c6da-102">Wiederherstellen eines gelöschten öffentlichen Ordners</span><span class="sxs-lookup"><span data-stu-id="3c6da-102">Restore a deleted public folder</span></span>

<span data-ttu-id="3c6da-103">**So stellen Sie gelöschte Elemente aus einem öffentlichen Ordner wieder auf:**</span><span class="sxs-lookup"><span data-stu-id="3c6da-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="3c6da-104">Weitere Informationen finden Sie unter Sie können gelöschte Elemente aus einem öffentlichen Ordner ohne [E-Mail in Outlook 2016 nicht wiederherstellen.](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="3c6da-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="3c6da-105">**So stellen Sie einen gelöschten öffentlichen Ordner (beliebigen Typs) wieder auf:**</span><span class="sxs-lookup"><span data-stu-id="3c6da-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="3c6da-106">Verwenden Sie den folgenden EXO PowerShell-Befehl:</span><span class="sxs-lookup"><span data-stu-id="3c6da-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="3c6da-107">Syntax:</span><span class="sxs-lookup"><span data-stu-id="3c6da-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="3c6da-108">Beispiel: Mit dem folgenden Befehl wird Subfolder1 wiederhergestellt und unter \Parent1 gespeichert:</span><span class="sxs-lookup"><span data-stu-id="3c6da-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="3c6da-109">Weitere [Informationen finden Sie unter Wiederherstellen eines gelöschten öffentlichen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Ordners.</span><span class="sxs-lookup"><span data-stu-id="3c6da-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
