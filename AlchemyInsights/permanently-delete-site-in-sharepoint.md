---
title: Endgültiges Löschen einer Site in SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771720"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="35cb6-102">Endgültiges Löschen einer Site in SharePoint</span><span class="sxs-lookup"><span data-stu-id="35cb6-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="35cb6-103">Um eine URL von einer gelöschten Site wiederzuverwenden (zum Neuerstellen einer Site) oder um eine Site endgültig zu löschen, weil sie nicht mehr verwendet wird, können Sie **Endgültig löschen** im neuen SharePoint Admin Center verwenden.</span><span class="sxs-lookup"><span data-stu-id="35cb6-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="35cb6-104">Wechseln Sie zur [Seite „Gelöschte Sites“ im neuen SharePoint Admin Center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true), und melden Sie sich mit einem Konto an, das über Administratorberechtigungen für Ihre Organisation verfügt.</span><span class="sxs-lookup"><span data-stu-id="35cb6-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="35cb6-105">Wählen Sie in der linken Spalte eine Site aus.</span><span class="sxs-lookup"><span data-stu-id="35cb6-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="35cb6-106">Klicken Sie auf **Endgültig löschen**.</span><span class="sxs-lookup"><span data-stu-id="35cb6-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="35cb6-107">**Hinweis**: Mit Gruppen verbundene Sites können über das neue SharePoint Admin Center nicht endgültig gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="35cb6-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="35cb6-108">Stattdessen müssen Sie [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) verwenden.</span><span class="sxs-lookup"><span data-stu-id="35cb6-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="35cb6-109">Weitere Informationen finden Sie unter [Endgültiges Löschen einer Site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="35cb6-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
