---
title: Erstellen einer SharePoint-Website
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806938"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="4b956-102">Erstellen einer SharePoint-Website</span><span class="sxs-lookup"><span data-stu-id="4b956-102">Create a SharePoint site</span></span>

<span data-ttu-id="4b956-103">Erstellen oder Verwalten von Websites von [aktiven Websites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) im SharePoint Admin Center.</span><span class="sxs-lookup"><span data-stu-id="4b956-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="4b956-104">Weitere Informationen finden Sie unter [Verwalten von Websites im neuen SharePoint Admin Center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4b956-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="4b956-105">Tipps</span><span class="sxs-lookup"><span data-stu-id="4b956-105">Tips:</span></span>

- <span data-ttu-id="4b956-106">Sie **können keine** Website mit derselben URL einer vorhandenen Website erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b956-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="4b956-107">Wenn Sie eine Website gelöscht haben und die URL erneut verwenden möchten, ist es möglich, dass die gelöschte Website weiterhin unter [Gelöschte Websites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4b956-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="4b956-108">Die Website muss endgültig gelöscht werden, damit die URL wieder verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="4b956-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="4b956-109">Informationen zum vollständigen Entfernen einer Website mit PowerShell finden Sie unter [Remove-SPSite-Cmdlet-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) Beispiel.</span><span class="sxs-lookup"><span data-stu-id="4b956-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="4b956-110">Einige Benutzer können möglicherweise keine Website erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b956-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="4b956-111">[Weitere Informationen finden Sie unter Manage Site Creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4b956-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="4b956-112">Möglicherweise wird die Website bei der **Erstellung** länger als erwartet blockiert.</span><span class="sxs-lookup"><span data-stu-id="4b956-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="4b956-113">Wenn seit dem ersten Auftreten dieses Problems mehr als 24 Stunden vergangen sind, melden Sie sich ein Support Ticket an.</span><span class="sxs-lookup"><span data-stu-id="4b956-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4b956-114">In vielen Fällen arbeiten wir bereits an einer Lösung.</span><span class="sxs-lookup"><span data-stu-id="4b956-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4b956-115">Geben Sie uns mindestens 24 Stunden, um eine Lösung zu vervollständigen.</span><span class="sxs-lookup"><span data-stu-id="4b956-115">Please give us at least 24 hours to complete a solution.</span></span>
