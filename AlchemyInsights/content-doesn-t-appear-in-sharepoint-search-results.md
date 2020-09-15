---
title: Inhalte werden nicht in SharePoint-Suchergebnissen angezeigt
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713129"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="07ae3-102">Inhalte werden nicht in SharePoint-Suchergebnissen angezeigt</span><span class="sxs-lookup"><span data-stu-id="07ae3-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="07ae3-103">Befolgen Sie diese Schritte zur Problembehandlung, wenn der erwartete Inhalt nicht in den Suchergebnissen angezeigt wird:</span><span class="sxs-lookup"><span data-stu-id="07ae3-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="07ae3-104">Stellen Sie sicher, dass die **Website** mit dem erwarteten Inhalt so festgelegt ist, dass Inhalte in den Suchergebnissen angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="07ae3-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="07ae3-105">Führen Sie die Schritte unter [Anzeigen von Inhalten auf einer Website in Suchergebnissen](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)aus.</span><span class="sxs-lookup"><span data-stu-id="07ae3-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="07ae3-106">Stellen Sie sicher, dass die **Liste** oder **Bibliothek** , die den erwarteten Inhalt enthält, so festgelegt ist, dass Inhalte in den Suchergebnissen angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="07ae3-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="07ae3-107">Führen Sie die Schritte unter [Anzeigen von Inhalten aus Listen oder Bibliotheken in Suchergebnissen aus](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="07ae3-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="07ae3-108">Stellen Sie sicher, dass das Seiten-, Dokument-oder benutzerdefinierte Seitenlayout als **Hauptversion** veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="07ae3-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="07ae3-109">Befolgen von Schritt 3 in der [Suche werden nicht alle Ergebnisse in SharePoint Online zurückgegeben](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="07ae3-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="07ae3-110">Stellen Sie sicher, dass der Benutzer über **Berechtigungen** zum Anzeigen des Inhalts verfügt.</span><span class="sxs-lookup"><span data-stu-id="07ae3-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="07ae3-111">Befolgen Sie die Schritte unter [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="07ae3-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="07ae3-112">Wenn das Suchschema durch Hinzufügen einer neuen verwalteten Eigenschaft, durch Bearbeiten einer verwalteten Eigenschaft oder durch Entfernen einer verwalteten Eigenschaft geändert wurde, müssen Sie eine Durchforstung und eine erneute Indizierung anfordern.</span><span class="sxs-lookup"><span data-stu-id="07ae3-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="07ae3-113">Führen Sie die Schritte unter [Manuelles anfordern des Durchforstens und erneuten Indizierens einer Website, einer Bibliothek oder einer Liste aus,](https://docs.microsoft.com/sharepoint/crawl-site-content)um den Inhalt **neu zu indizieren** .</span><span class="sxs-lookup"><span data-stu-id="07ae3-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="07ae3-114">Dies kann eine Weile dauern, warten Sie 24 Stunden, bevor Sie die Ergebnisse erneut überprüfen.</span><span class="sxs-lookup"><span data-stu-id="07ae3-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="07ae3-115">Weitere Informationen finden Sie unter [Aktivieren des Inhalts einer Website, um durchsuchbar zu sein](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="07ae3-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
