---
title: eDiscovery-Exporttool
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814587"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="e48a4-102">Kann das eDiscovery-Exporttool nicht installiert oder ausgeführt werden?</span><span class="sxs-lookup"><span data-stu-id="e48a4-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="e48a4-103">Wenn Sie das eDiscovery-Exporttool nicht installieren oder ausführen können, um Suchergebnisse herunterzuladen, überprüfen Sie folgendes:</span><span class="sxs-lookup"><span data-stu-id="e48a4-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="e48a4-104">Der computer, den Sie verwenden, erfüllt die folgenden Voraussetzungen:</span><span class="sxs-lookup"><span data-stu-id="e48a4-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="e48a4-105">32- oder 64-Bit-Versionen von Windows 7 und höher</span><span class="sxs-lookup"><span data-stu-id="e48a4-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="e48a4-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="e48a4-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="e48a4-107">Einen unterstützten Browser:</span><span class="sxs-lookup"><span data-stu-id="e48a4-107">A supported browser:</span></span>

  - <span data-ttu-id="e48a4-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e48a4-108">Microsoft Edge</span></span>

    <span data-ttu-id="e48a4-109">Oder</span><span class="sxs-lookup"><span data-stu-id="e48a4-109">Or</span></span>

  - <span data-ttu-id="e48a4-110">Internet Explorer 10 und höher</span><span class="sxs-lookup"><span data-stu-id="e48a4-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="e48a4-111">Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e48a4-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="e48a4-112">Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, der **\* .blob.core.windows.net** ist (der Platzhalter stellt einen eindeutigen Bezeichner für Ihren Exportauftrag dar).</span><span class="sxs-lookup"><span data-stu-id="e48a4-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="e48a4-113">Ihnen wird die Rolle Export im Microsoft 365 Security &amp; Compliance Center zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e48a4-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="e48a4-114">Diese Rolle wird standardmäßig nur der Rollengruppe eDiscovery Manager zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e48a4-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="e48a4-115">Weitere [Informationen finden Sie unter Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="e48a4-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="e48a4-116">Weitere Informationen finden Sie unter [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="e48a4-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="e48a4-117">Wenn Sie mehr als 100.000-Postfächer exportieren, müssen Sie die folgenden Powershell verwenden, um die Exportergebnisse herunterzuladen: Exportieren von Ergebnissen aus mehr als  [100-K-Postfächern](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="e48a4-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>