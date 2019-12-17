---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068400"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="dd74d-102">SharePoint oder OneDrive langsam, unzugänglich oder nicht verfügbar für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="dd74d-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="dd74d-103">SharePoint oder OneDrive ist möglicherweise langsam, unzugänglich oder nicht verfügbar oder kann Dienst nicht verfügbar oder 503-Fehler aus mehreren Gründen anzeigen:</span><span class="sxs-lookup"><span data-stu-id="dd74d-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="dd74d-104">Wenn Ihre SharePoint-oder OneDrive-Website für mehrere Benutzer langsam oder verzögert ist, gibt es möglicherweise ein vorübergehendes Dienst Problem, bei dem Benutzer bei Zugriff auf SharePoint-Websites oder OneDrive-Inhalte zeitweilig Verzögerungen oder Navigationsfehler auftreten.</span><span class="sxs-lookup"><span data-stu-id="dd74d-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="dd74d-105">Überprüfen Sie das [Dienststatus-Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , um zu sehen, ob Ihre Organisation betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="dd74d-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="dd74d-106">Bei dem Versuch, zu SharePoint-oder OneDrive-Websites zu navigieren, erhalten Benutzer möglicherweise einen Fehler " *503 Server ist ausgelastet* ".</span><span class="sxs-lookup"><span data-stu-id="dd74d-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="dd74d-107">Dieser Fehler kann durch Drosselung im SharePoint-Dienst verursacht werden.</span><span class="sxs-lookup"><span data-stu-id="dd74d-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="dd74d-108">SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten.</span><span class="sxs-lookup"><span data-stu-id="dd74d-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="dd74d-109">Einschränkungsgrenzwerte Ruft die Anzahl von Aktionen eines Benutzers oder gleichzeitige (von Code- oder Skriptblock), um Ressourcen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="dd74d-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="dd74d-110">Weitere Informationen zur Drosselung finden Sie unter vermeiden Sie eine [Drosselung oder Blockierung in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="dd74d-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="dd74d-111">Wenn Sie eine langsame Leistung mit einer **klassischen** oder **modernen** SharePoint-Website oder-Seite erleben, verwenden Sie das Seiten [Diagnosetool](https://aka.ms/perftool) , um die Seiten zu analysieren.</span><span class="sxs-lookup"><span data-stu-id="dd74d-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="dd74d-112">Wenn Sie weiterhin eine allgemeine langsame Leistung erzielen, lesen Sie die Ressourcen unten in diesem Artikel: [Einführung in die Leistungsoptimierung für SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="dd74d-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  