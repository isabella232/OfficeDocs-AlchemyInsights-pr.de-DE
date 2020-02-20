---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158500"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="9709a-102">Wiederherstellen eines gelöschten öffentlichen Ordners</span><span class="sxs-lookup"><span data-stu-id="9709a-102">Restore a deleted public folder</span></span>

<span data-ttu-id="9709a-103">**So stellen Sie gelöschte Elemente in einem öffentlichen Ordner wieder her**:</span><span class="sxs-lookup"><span data-stu-id="9709a-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="9709a-104">Weitere Informationen finden [Sie unter Sie können gelöschte Elemente nicht aus einem öffentlichen Ordner außerhalb von e-Mail in Outlook 2016 wiederherstellen](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="9709a-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="9709a-105">**So stellen Sie einen gelöschten öffentlichen Ordner (eines beliebigen Typs) wieder her**:</span><span class="sxs-lookup"><span data-stu-id="9709a-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="9709a-106">Verwenden Sie den folgenden Exo PowerShell-Befehl:</span><span class="sxs-lookup"><span data-stu-id="9709a-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="9709a-107">Syntax:</span><span class="sxs-lookup"><span data-stu-id="9709a-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="9709a-108">Beispiel: mit dem folgenden Befehl wird Unterordner1 wiederhergestellt und unter \Parent1 platziert:</span><span class="sxs-lookup"><span data-stu-id="9709a-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="9709a-109">Weitere Informationen finden Sie unter [Wiederherstellen eines gelöschten öffentlichen Ordners](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="9709a-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
