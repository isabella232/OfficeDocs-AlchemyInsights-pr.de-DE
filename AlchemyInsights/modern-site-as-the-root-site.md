---
title: Moderne Website als Stammwebsite
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057711"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="a0528-102">Moderne Website als Stammwebsite</span><span class="sxs-lookup"><span data-stu-id="a0528-102">Modern site as root site</span></span>

<span data-ttu-id="a0528-103">[Ziel Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) -Kunden können jetzt die moderne Kommunikationswebsite auf der klassischen Stammwebsite Ihres SharePoint-Mandanten aktivieren.</span><span class="sxs-lookup"><span data-stu-id="a0528-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="a0528-104">Dieses Feature kann durch Ausführen eines einfachen PowerShell-Cmdlets aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="a0528-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="a0528-105">Bei erfolgreicher Ausführung der PowerShell-Befehle verfügt die Stammwebsite über eine neue Homepage für die Kommunikationswebsite.</span><span class="sxs-lookup"><span data-stu-id="a0528-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="a0528-106">Details zu den PowerShell-Cmdlets und Funktionsanforderungen finden Sie im Artikel [enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="a0528-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="a0528-107">Nach und nach werden wir das in der Standardeinstellung für Zielversionen von Kunden Anfang Mai 2019 und die Einführung weltweit bis Ende Juni 2019 zur Verfügung stellen.</span><span class="sxs-lookup"><span data-stu-id="a0528-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="a0528-108">Weitere Informationen finden Sie im [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) für andere neue Features mit modern.</span><span class="sxs-lookup"><span data-stu-id="a0528-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="a0528-109">**Wichtig**: Löschen Sie Ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="a0528-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="a0528-110">Dies wird von Microsoft nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0528-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="a0528-111">Durch das Löschen der Stammwebsite werden alle SharePoint-Websites in Ihrer Organisation für alle Benutzer unzugänglich, bis Sie die Website wiederherstellen oder eine neue Website mit derselben URL erstellen.</span><span class="sxs-lookup"><span data-stu-id="a0528-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 