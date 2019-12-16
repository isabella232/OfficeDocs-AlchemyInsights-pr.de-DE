---
title: Erstellen einer SharePoint-Website
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 2611c3ed9cfe78c82c9b123ea26b6fe8f951b458
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049876"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="bb44a-102">Erstellen einer SharePoint-Website</span><span class="sxs-lookup"><span data-stu-id="bb44a-102">Create a SharePoint site</span></span>

<span data-ttu-id="bb44a-103">Informationen zur Erstellung von SharePoint-Websites finden Sie im folgenden:</span><span class="sxs-lookup"><span data-stu-id="bb44a-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="bb44a-104">[Verwalten von Websites im neuen SharePoint Admin Center](https://docs.microsoft.com/sharepoint/manage-site-creation): Informationen zu Website Erstellungsoptionen, einschließlich der Vorgehensweise zum Erstellen einer klassischen Website oder einer Microsoft Teams-Website, die keine Office 365 Gruppe enthält.</span><span class="sxs-lookup"><span data-stu-id="bb44a-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="bb44a-105">[Erstellen einer Teamwebsite in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Hier erfahren Sie, wie Sie eine Teamwebsite erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb44a-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="bb44a-106">[Erstellen Sie eine Kommunikationswebsite in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): erfahren Sie, wie Sie eine Kommunikationswebsite erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb44a-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="bb44a-107">[Verwalten von Websites im neuen SharePoint Admin Center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Hier erfahren Sie, wie Sie eine klassische Website oder eine Teamwebsite erstellen, die keine Office 365 Gruppe enthält.</span><span class="sxs-lookup"><span data-stu-id="bb44a-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="bb44a-108">**Tipps**</span><span class="sxs-lookup"><span data-stu-id="bb44a-108">**Tips:**</span></span>
- <span data-ttu-id="bb44a-109">Sie können keine Website mit derselben URL einer vorhandenen Website erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb44a-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="bb44a-110">Wenn Sie eine Website gelöscht haben und die URL erneut verwenden möchten, ist es möglich, dass die gelöschte Website weiterhin unter **Gelöschte Websites**vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="bb44a-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="bb44a-111">Informationen zum Verwalten gelöschter Websites finden Sie unter [Löschen einer Website](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="bb44a-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="bb44a-112">Informationen zum vollständigen Entfernen einer Website mit PowerShell finden Sie unter [Remove-SPSite-Cmdlet-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) Beispiel.</span><span class="sxs-lookup"><span data-stu-id="bb44a-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="bb44a-113">Einige Benutzer können möglicherweise keine Website erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb44a-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="bb44a-114">Weitere Informationen finden Sie unter [Manage Site Creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bb44a-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="bb44a-115">Möglicherweise wird die Website bei der **Erstellung** länger als erwartet blockiert.</span><span class="sxs-lookup"><span data-stu-id="bb44a-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="bb44a-116">Wenn seit dem ersten Auftreten dieses Problems mehr als 24 Stunden vergangen sind, melden Sie sich ein Support Ticket an.</span><span class="sxs-lookup"><span data-stu-id="bb44a-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="bb44a-117">In vielen Fällen arbeiten wir bereits an einer Lösung.</span><span class="sxs-lookup"><span data-stu-id="bb44a-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="bb44a-118">Geben Sie uns mindestens 24 Stunden, um eine Lösung zu vervollständigen.</span><span class="sxs-lookup"><span data-stu-id="bb44a-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="bb44a-119">Wenn Sie eine neue Teamwebsite erstellen müssen, die keine Office 365 Gruppe enthält,</span><span class="sxs-lookup"><span data-stu-id="bb44a-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


