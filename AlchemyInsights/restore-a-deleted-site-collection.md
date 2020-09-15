---
title: Wiederherstellen einer gelöschten Website
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692042"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="9823e-102">Wiederherstellen einer gelöschten Website</span><span class="sxs-lookup"><span data-stu-id="9823e-102">Restore a deleted site</span></span>

<span data-ttu-id="9823e-103">Wenn ein Administrator eine SharePoint-Website löscht, wird er im Papierkorb der Websitesammlung abgelegt, wo er für 93 Tage aufbewahrt wird, bevor er endgültig gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="9823e-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="9823e-104">So stellen Sie die Website wieder her:</span><span class="sxs-lookup"><span data-stu-id="9823e-104">To restore the site:</span></span>
  
1. <span data-ttu-id="9823e-105">Klicken Sie im neuen SharePoint Admin Center auf dem Menüband auf **Papierkorb** .</span><span class="sxs-lookup"><span data-stu-id="9823e-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="9823e-106">Aktivieren Sie das Kontrollkästchen neben der Websitesammlung, die Sie wiederherstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="9823e-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="9823e-107">Klicken Sie auf **Gelöschte Elemente wiederherstellen**.</span><span class="sxs-lookup"><span data-stu-id="9823e-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="9823e-108">Zum Wiederherstellen einer gelöschten Kommunikationswebsite können Sie das neue SharePoint Admin Center verwenden.</span><span class="sxs-lookup"><span data-stu-id="9823e-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="9823e-109">Andernfalls müssen Sie Microsoft PowerShell verwenden.</span><span class="sxs-lookup"><span data-stu-id="9823e-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="9823e-110">Zum Wiederherstellen einer Website, die zu einer Microsoft 365-Gruppe gehört, müssen Sie die Gruppe im Exchange Admin Center wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="9823e-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="9823e-111">Gruppen können 30 Tage nach dem Löschen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="9823e-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

