---
title: Moderne Website als Stammwebsite
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620758"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="1b344-102">Moderne Website als Stammwebsite</span><span class="sxs-lookup"><span data-stu-id="1b344-102">Modern site as root site</span></span>

<span data-ttu-id="1b344-103">Wir haben mit dem Rollout eines neuen Features begonnen, mit dem Sie Ihre klassische Websitestamm Website mit einer modernen Website austauschen können.</span><span class="sxs-lookup"><span data-stu-id="1b344-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="1b344-104">Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , um den Speicherort einer Website während der Archivierung der ursprünglichen Website mit einer anderen Website zu vertauschen.</span><span class="sxs-lookup"><span data-stu-id="1b344-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1b344-105">Für beide Team Websites (nicht verbunden mit einer Gruppe) und Kommunikationswebsite verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1b344-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="1b344-106">Löschen Sie Ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b344-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="1b344-107">Dies wird von Microsoft nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b344-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="1b344-108">Wenn Sie die Stammwebsite löschen, können alle SharePoint-Websites in Ihrer Organisation erst für alle Benutzer zugänglich gemacht werden, wenn Sie die Website wiederherstellen oder eine neue Website mit derselben URL erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b344-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="1b344-109">Diese Funktion wird über das Nachrichtencenter kommuniziert.</span><span class="sxs-lookup"><span data-stu-id="1b344-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="1b344-110">Sie sollten davon ausgehen, dass das Feature in Ihrem Mandanten in Kürze aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="1b344-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1b344-111">Bekannte Probleme beim Austauschen von Websites</span><span class="sxs-lookup"><span data-stu-id="1b344-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="1b344-112">Die Zielwebsite gibt möglicherweise einen Fehler "nicht gefunden" (HTTP 404) für eine kurze Zeit zurück.</span><span class="sxs-lookup"><span data-stu-id="1b344-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1b344-113">Der Inhalt muss erneut durchforstet werden, um den Suchindex zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="1b344-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1b344-114">Es ist kein manueller Schritt erforderlich, dies erfolgt automatisch.</span><span class="sxs-lookup"><span data-stu-id="1b344-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="1b344-115">Alles, was von "statischen" Links (wie Dateisynchronisierung und OneNote-Dateien) abhängig ist, muss manuell korrigiert werden.</span><span class="sxs-lookup"><span data-stu-id="1b344-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1b344-116">Project Server-Websites müssen möglicherweise überprüft werden, um sicherzustellen, dass Sie weiterhin ordnungsgemäß zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="1b344-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
