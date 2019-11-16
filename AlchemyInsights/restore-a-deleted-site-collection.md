---
title: Wiederherstellen einer gelöschten Website
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768547"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="e9b83-102">Wiederherstellen einer gelöschten Website</span><span class="sxs-lookup"><span data-stu-id="e9b83-102">Restore a deleted site</span></span>

<span data-ttu-id="e9b83-103">Wenn ein Administrator eine SharePoint-Website löscht, wird er im Papierkorb der Websitesammlung abgelegt, wo er für 93 Tage aufbewahrt wird, bevor er endgültig gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="e9b83-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="e9b83-104">So stellen Sie die Website wieder her:</span><span class="sxs-lookup"><span data-stu-id="e9b83-104">To restore the site:</span></span>
  
1. <span data-ttu-id="e9b83-105">Klicken Sie im neuen SharePoint Admin Center auf dem Menüband auf **Papierkorb** .</span><span class="sxs-lookup"><span data-stu-id="e9b83-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="e9b83-106">Aktivieren Sie das Kontrollkästchen neben der Websitesammlung, die Sie wiederherstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="e9b83-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="e9b83-107">Klicken Sie auf **Gelöschte Elemente wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="e9b83-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="e9b83-108">Zum Wiederherstellen einer gelöschten Kommunikationswebsite können Sie das neue SharePoint Admin Center verwenden.</span><span class="sxs-lookup"><span data-stu-id="e9b83-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="e9b83-109">Andernfalls müssen Sie Microsoft PowerShell verwenden.</span><span class="sxs-lookup"><span data-stu-id="e9b83-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="e9b83-110">Zum Wiederherstellen einer Website, die zu einer Office 365 Gruppe gehört, müssen Sie die Gruppe im Exchange Admin Center wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="e9b83-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="e9b83-111">Gruppen können 30 Tage nach dem Löschen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e9b83-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

