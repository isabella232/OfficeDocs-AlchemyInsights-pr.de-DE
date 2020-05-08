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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064392"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="31757-102">Probleme beim Erstellen einer mit einer Gruppe verbundenen Website in SharePoint</span><span class="sxs-lookup"><span data-stu-id="31757-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="31757-103">Einige häufige Probleme, die beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen auftreten.</span><span class="sxs-lookup"><span data-stu-id="31757-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="31757-104">Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.</span><span class="sxs-lookup"><span data-stu-id="31757-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="31757-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="31757-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="31757-106">Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="31757-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="31757-107">Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites.</span><span class="sxs-lookup"><span data-stu-id="31757-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="31757-108">PowerShell ist erforderlich, um Gruppen Websites endgültig zu löschen.</span><span class="sxs-lookup"><span data-stu-id="31757-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="31757-109">Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten: **bereits eine andere Gruppe mit demselben Alias vorhanden**ist, überprüfen Sie die vorhandenen Gruppen im [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="31757-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="31757-110">Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="31757-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="31757-111">Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="31757-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="31757-112">Sie können vorhandene Websites mit einer Microsoft 365-Gruppe verbinden.</span><span class="sxs-lookup"><span data-stu-id="31757-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="31757-113">Weitere Informationen finden Sie unter [Verbinden einer Microsoft 365-Gruppe mithilfe der SharePoint-Benutzeroberfläche](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="31757-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="31757-114">Um eine verbundene Website der Microsoft 365-Gruppe zu erstellen, müssen Sie eine [Team Website](https://admin.microsoft.com/sharepoint)erstellen.</span><span class="sxs-lookup"><span data-stu-id="31757-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
