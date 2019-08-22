---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507846"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="efb45-102">Probleme beim Erstellen oder gruppieren verbundener Websites in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="efb45-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="efb45-103">Beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen sind einige häufige Probleme aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="efb45-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="efb45-104">Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.</span><span class="sxs-lookup"><span data-stu-id="efb45-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="efb45-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="efb45-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="efb45-106">Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="efb45-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="efb45-107">Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites.</span><span class="sxs-lookup"><span data-stu-id="efb45-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="efb45-108">Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten, dass bereits eine andere Gruppe mit demselben Alias vorhanden ist, überprüfen Sie die vorhandenen Gruppen aus dem [Office 365 aus dem Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="efb45-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="efb45-109">Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="efb45-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="efb45-110">Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="efb45-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="efb45-111">Sie können vorhandene Websites mit einer Office 365 Gruppe verbinden.</span><span class="sxs-lookup"><span data-stu-id="efb45-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="efb45-112">Weitere Informationen finden Sie unter [Verbinden einer Office 365 Gruppe mit dem SharePoint-Benutzer ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="efb45-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="efb45-113">Um eine verbundene Website mit Office 365 Gruppe zu erstellen, müssen Sie eine Team Website erstellen.</span><span class="sxs-lookup"><span data-stu-id="efb45-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="efb45-114">Weitere Informationen finden Sie unter [Erstellen einer Teamwebsite in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="efb45-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

