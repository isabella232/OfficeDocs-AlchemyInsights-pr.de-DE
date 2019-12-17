---
title: Verwalten des Suchschemas in SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042962"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="257a8-102">Verwalten des Suchschemas in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="257a8-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="257a8-103">Das Suchschema steuert, was Benutzer suchen können, wie Benutzer Sie durchsuchen können und wie Sie die Ergebnisse auf Ihren suchwebsites präsentieren können.</span><span class="sxs-lookup"><span data-stu-id="257a8-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="257a8-104">Informationen zur folgenden Vorgehensweise finden Sie unter [Verwalten des Suchschemas in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) :</span><span class="sxs-lookup"><span data-stu-id="257a8-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="257a8-105">Ändern Sie das Suchschema.</span><span class="sxs-lookup"><span data-stu-id="257a8-105">Change the search schema.</span></span>
- <span data-ttu-id="257a8-106">Erstellen verwalteter Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="257a8-106">Create managed properties.</span></span>
- <span data-ttu-id="257a8-107">Durchforstete Map durchforstete Eigenschaften zu verwalteten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="257a8-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="257a8-108">Beachten Sie Folgendes in Bezug auf die Verwaltung Ihres Suchschemas:</span><span class="sxs-lookup"><span data-stu-id="257a8-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="257a8-109">Wenn Sie eine Warnung erhalten, die besagt, dass **die Anwendung angehalten** wurde, wenn eine Schemaänderung vorgenommen wird, ist dies nur temporär, da die Wartung des Diensts ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="257a8-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="257a8-110">Wenn mehr als 24 Stunden vergangen sind und Sie weiterhin die Warnung erhalten, melden Sie sich bitte bei einem Supportfall an.</span><span class="sxs-lookup"><span data-stu-id="257a8-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="257a8-111">Wenn Sie verwaltete Eigenschaften ändern oder neue hinzufügen, werden die Änderungen erst wirksam, nachdem der Inhalt erneut durchforstet wurde.</span><span class="sxs-lookup"><span data-stu-id="257a8-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="257a8-112">In SharePoint Online erfolgt das Crawlen automatisch basierend auf dem definierten durchforstungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="257a8-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="257a8-113">Um sicherzustellen, dass Ihre Änderungen gecrawlt werden, können Sie [eine erneute Indizierung der Liste oder Bibliothek anfordern](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="257a8-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="257a8-114">Eine vollständige Übersicht über das Suchschema finden Sie unter Einführung in das [Suchschema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="257a8-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


