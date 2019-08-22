---
title: Suchen in SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507630"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="cfa91-102">Durchforsten und Indizieren von Inhalten in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cfa91-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="cfa91-103">Inhalte müssen durchforstet und dem Suchindex hinzugefügt werden, damit Benutzer in SharePoint Online nach Ihren Suchvorgängen suchen können.</span><span class="sxs-lookup"><span data-stu-id="cfa91-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="cfa91-104">Der Inhalt wird automatisch basierend auf einem vordefinierten durchforstungszeitplan gecrawlt (der durchforstungszeitplan kann nicht geändert werden).</span><span class="sxs-lookup"><span data-stu-id="cfa91-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="cfa91-105">Der Crawler ruft Inhalte ab, die seit der letzten Durchforstung geändert wurden, und aktualisiert den Index.</span><span class="sxs-lookup"><span data-stu-id="cfa91-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="cfa91-106">Wenn Sie sicherstellen möchten, dass Inhalt gecrawlt wird und der Index aktualisiert wird, beachten Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="cfa91-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="cfa91-107">Stellen Sie sicher, dass Inhalte gefunden werden können, indem [Websiteinhalte durchsuchbar gemacht](https://docs.microsoft.com/sharepoint/make-site-content-searchable)werden.</span><span class="sxs-lookup"><span data-stu-id="cfa91-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="cfa91-108">Wenn Sie eine verwaltete Eigenschaft geändert oder die Zuordnung von durchforstete und verwalteten Eigenschaften geändert haben, muss die Website erneut durchforstet werden, bevor Ihre Änderungen im Suchindex wiedergegeben werden.</span><span class="sxs-lookup"><span data-stu-id="cfa91-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="cfa91-109">Da Ihre Änderungen im Suchschema und nicht auf der tatsächlichen Website vorgenommen werden, wird die Website vom Crawler nicht automatisch neu indiziert.</span><span class="sxs-lookup"><span data-stu-id="cfa91-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="cfa91-110">Weitere Informationen finden Sie unter [Manuelles anfordern der Durchforstung und erneuten Indizierung einer Website, einer Bibliothek oder einer Liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="cfa91-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="cfa91-111">Warten Sie mindestens 24 Stunden nach der manuellen Anforderung einer Durchforstung und der vollständigen erneuten Indizierung, um zu sehen, ob noch ein Problem auftritt.</span><span class="sxs-lookup"><span data-stu-id="cfa91-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="cfa91-112">Wenn seit dem Initiieren der Durchforstung und der vollständigen erneuten Indizierung mehr als 24 Stunden vergangen sind, melden Sie sich einen Supportfall an.</span><span class="sxs-lookup"><span data-stu-id="cfa91-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="cfa91-113">In vielen Fällen arbeiten wir bereits an einer Lösung.</span><span class="sxs-lookup"><span data-stu-id="cfa91-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="cfa91-114">Geben Sie uns mindestens 24 Stunden, um eine Lösung zu vervollständigen.</span><span class="sxs-lookup"><span data-stu-id="cfa91-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cfa91-115">Wenn eine Website, ein Dokument (Bibliothek) oder eine Liste gelöscht wurde und weiterhin in den Suchergebnissen angezeigt wird, sollten Benutzer eine **Fehler 404-Datei** erhalten, die nicht gefunden wurde, wenn Sie versuchen, darauf zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="cfa91-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="cfa91-116">Dieses Problem sollte bei weiteren Untersuchungen als Supportfall protokolliert werden.</span><span class="sxs-lookup"><span data-stu-id="cfa91-116">This issue should be logged as a support case for further investigation.</span></span> 



