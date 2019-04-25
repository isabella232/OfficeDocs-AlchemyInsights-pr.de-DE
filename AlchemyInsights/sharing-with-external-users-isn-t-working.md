---
title: Freigabe für externe Benutzer funktioniert nicht
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369497"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="291a2-102">Beheben von Problemen beim Freigeben von SharePoint-Inhalten für externe Benutzer</span><span class="sxs-lookup"><span data-stu-id="291a2-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="291a2-103">Stellen Sie sicher, dass die externe Freigabe für Ihre Organisation aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="291a2-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="291a2-104">Wechseln Sie zur [Seite &amp; Dienste-Add-ins im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), und klicken Sie auf **Websites**.</span><span class="sxs-lookup"><span data-stu-id="291a2-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="291a2-105">Stellen Sie sicher, dass die Einstellung auf "ein" aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="291a2-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="291a2-106">Wenn "nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer im Microsoft 365 Admin Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="291a2-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="291a2-107">Stellen Sie sicher, dass die externe Freigabe für die Website aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="291a2-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="291a2-108">Für eine klassische Websitesammlung:</span><span class="sxs-lookup"><span data-stu-id="291a2-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="291a2-109">Klicken Sie im neuen SharePoint Admin Center im linken Bereich auf **Websites**.</span><span class="sxs-lookup"><span data-stu-id="291a2-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="291a2-110">Wählen Sie die Website oder Websites aus, und klicken Sie auf dem Menüband auf **Freigabe**.</span><span class="sxs-lookup"><span data-stu-id="291a2-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="291a2-111">Für eine Teamwebsite, die zu einer Office 365-Gruppe oder einer Kommunikationswebsite gehört:</span><span class="sxs-lookup"><span data-stu-id="291a2-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="291a2-112">Diese neuen Websitetypen haben dieselbe Freigabe Einstellung wie Ihre organisationsweite Einstellung, es sei denn, die organisationsweite Einstellung ermöglicht das Freigeben von Dateien mit Links, die keine Anmeldung erfordern.</span><span class="sxs-lookup"><span data-stu-id="291a2-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="291a2-113">In diesem Fall ermöglichen die Websites die Freigabe für neue und vorhandene externe Benutzer, die sich anmelden.</span><span class="sxs-lookup"><span data-stu-id="291a2-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="291a2-114">Um die Einstellung für bestimmte Websites zu ändern, verwenden Sie das neue SharePoint Admin Center oder die PowerShell.</span><span class="sxs-lookup"><span data-stu-id="291a2-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="291a2-115">[Weitere Informationen](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="291a2-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="291a2-116">Die Einstellung für die externe Freigabe für jede Website kann restriktiver sein als die organisationsweite Einstellung, aber nicht mehr als die organisationsweite Einstellung.</span><span class="sxs-lookup"><span data-stu-id="291a2-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

