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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063652"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="85180-102">Wiederherstellen eines gelöschten öffentlichen Ordners</span><span class="sxs-lookup"><span data-stu-id="85180-102">Restore a deleted public folder</span></span>

<span data-ttu-id="85180-103">**So stellen Sie gelöschte Elemente in einem öffentlichen Ordner wieder her**:</span><span class="sxs-lookup"><span data-stu-id="85180-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="85180-104">Weitere Informationen finden [Sie unter Sie können gelöschte Elemente nicht aus einem öffentlichen Ordner außerhalb von e-Mail in Outlook 2016 wiederherstellen](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="85180-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="85180-105">**So stellen Sie einen gelöschten öffentlichen Ordner (eines beliebigen Typs) wieder her**:</span><span class="sxs-lookup"><span data-stu-id="85180-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="85180-106">Verwenden Sie den folgenden Exo PowerShell-Befehl:</span><span class="sxs-lookup"><span data-stu-id="85180-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="85180-107">Syntax:</span><span class="sxs-lookup"><span data-stu-id="85180-107">Syntax:</span></span>

    ><span data-ttu-id="85180-108">$PF = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Rekursion |? {$_. Name-EQ "\<name_of_deleted_public_Folder"}; Festlegen-PublicFolder $PF. Identity-Path \<-Pfad, in dem der Ordner wiederhergestellt wird></span><span class="sxs-lookup"><span data-stu-id="85180-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="85180-109">Beispiel: mit dem folgenden Befehl wird Unterordner1 wiederhergestellt und unter \Parent1 platziert:</span><span class="sxs-lookup"><span data-stu-id="85180-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="85180-110">$PF = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Rekursion |? {$_. Name-EQ "Unterordner1"}; Gruppe-PublicFolder $PF. Identity-Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="85180-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="85180-111">Weitere Informationen finden Sie unter [Wiederherstellen eines gelöschten öffentlichen Ordners](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="85180-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
