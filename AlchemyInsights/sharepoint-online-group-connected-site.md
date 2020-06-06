---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582810"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="41a21-102">Probleme beim Erstellen einer mit einer Gruppe verbundenen Website in SharePoint</span><span class="sxs-lookup"><span data-stu-id="41a21-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="41a21-103">Einige häufige Probleme, die beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen auftreten.</span><span class="sxs-lookup"><span data-stu-id="41a21-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="41a21-104">Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.</span><span class="sxs-lookup"><span data-stu-id="41a21-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="41a21-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="41a21-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="41a21-106">Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="41a21-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="41a21-107">Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites.</span><span class="sxs-lookup"><span data-stu-id="41a21-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="41a21-108">PowerShell ist erforderlich, um Gruppen Websites endgültig zu löschen.</span><span class="sxs-lookup"><span data-stu-id="41a21-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="41a21-109">Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten: **bereits eine andere Gruppe mit demselben Alias vorhanden**ist, überprüfen Sie die vorhandenen Gruppen im [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="41a21-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="41a21-110">Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="41a21-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="41a21-111">Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="41a21-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="41a21-112">Sie können vorhandene Websites mit einer Microsoft 365-Gruppe verbinden.</span><span class="sxs-lookup"><span data-stu-id="41a21-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="41a21-113">Weitere Informationen finden Sie unter [Verbinden einer Microsoft 365-Gruppe mithilfe der SharePoint-Benutzeroberfläche](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="41a21-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="41a21-114">Um eine verbundene Website der Microsoft 365-Gruppe zu erstellen, müssen Sie eine [Team Website](https://admin.microsoft.com/sharepoint)erstellen.</span><span class="sxs-lookup"><span data-stu-id="41a21-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
