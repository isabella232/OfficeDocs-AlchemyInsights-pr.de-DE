---
title: Freigabe für externe Benutzer ist nicht funktionsfähig
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469890"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="eceac-102">Beheben von Problemen, die gemeinsame Nutzung von SharePoint-Inhalten mit externen Benutzern</span><span class="sxs-lookup"><span data-stu-id="eceac-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="eceac-103">Stellen Sie sicher, dass externe Freigabe für Ihre Organisation aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="eceac-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="eceac-104">Wechseln Sie zu der [Services &amp; Seite im Office 365 Administrationscenter-add-ins](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), und klicken Sie auf **Sites**.</span><span class="sxs-lookup"><span data-stu-id="eceac-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="eceac-p101">Stellen Sie sicher, dass die Einstellung auf "Aktiviert" aktiviert ist Wenn "Nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer in Office 365 Administrationscenter aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="eceac-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="eceac-p102">Stellen Sie sicher, dass externe Freigabe für die Website aktiviert. Für eine klassische Websitesammlung:</span><span class="sxs-lookup"><span data-stu-id="eceac-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="eceac-109">Klicken Sie in der klassischen SharePoint-Verwaltungskonsole im linken Bereich auf **Websitesammlungen**.</span><span class="sxs-lookup"><span data-stu-id="eceac-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="eceac-110">Wählen Sie die Website oder Websites, und klicken Sie auf dem Menüband auf **Freigabe**.</span><span class="sxs-lookup"><span data-stu-id="eceac-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="eceac-111">Für eine Teamwebsite, zu der eine Office 365-Gruppe gehört, oder eine Kommunikation-Website:</span><span class="sxs-lookup"><span data-stu-id="eceac-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="eceac-p103">Diese neuen Websitetypen haben die gleiche sharing festlegen als Ihrer Organisation geltende Einstellung, wenn die Einstellung der gesamten Organisation erlaubt die Freigabe von Dateien mithilfe von Links, die Anmeldung nicht erforderlich ist. In diesem Fall können die Websites mit neuen und vorhandenen externen Benutzern, die Anmeldung nutzt. Um die Einstellung für bestimmte Standorte zu ändern, verwenden Sie die neue SharePoint Administrationscenter (Preview) oder über PowerShell. [Erfahren Sie mehr](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="eceac-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="eceac-116">Die externe Freigabe für jede Website können restriktiver als Ihrer Organisation geltende Einstellung, aber nicht mehr als die Einstellung der gesamten Organisation permissive festgelegt.</span><span class="sxs-lookup"><span data-stu-id="eceac-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

