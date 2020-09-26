---
title: eDiscovery-Export Tool
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277923"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="97f44-102">Kann das eDiscovery-Export Tool nicht installiert oder ausgeführt werden?</span><span class="sxs-lookup"><span data-stu-id="97f44-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="97f44-103">Wenn Sie das eDiscovery-Export Tool zum Herunterladen von Suchergebnissen nicht installieren oder ausführen können, überprüfen Sie die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="97f44-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="97f44-104">Der verwendete Computer erfüllt die folgenden Voraussetzungen:</span><span class="sxs-lookup"><span data-stu-id="97f44-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="97f44-105">32- oder 64-Bit-Versionen von Windows 7 und höher</span><span class="sxs-lookup"><span data-stu-id="97f44-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="97f44-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="97f44-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="97f44-107">Einen unterstützten Browser:</span><span class="sxs-lookup"><span data-stu-id="97f44-107">A supported browser:</span></span>

  - <span data-ttu-id="97f44-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="97f44-108">Microsoft Edge</span></span>

    <span data-ttu-id="97f44-109">Oder:</span><span class="sxs-lookup"><span data-stu-id="97f44-109">Or</span></span>

  - <span data-ttu-id="97f44-110">Internet Explorer 10 und höher</span><span class="sxs-lookup"><span data-stu-id="97f44-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="97f44-111">Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97f44-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="97f44-112">Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, also \*\* \* . BLOB.Core.Windows.net\*\* (der Platzhalter stellt einen eindeutigen Bezeichner für den Exportauftrag dar).</span><span class="sxs-lookup"><span data-stu-id="97f44-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="97f44-113">Sie haben die Rolle Export im Microsoft 365 Security &amp; Compliance Center zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="97f44-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="97f44-114">Diese Rolle wird standardmäßig nur der Rollengruppe "eDiscovery-Manager" zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="97f44-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="97f44-115">Weitere Informationen finden Sie unter [Zuweisen von eDiscovery-Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="97f44-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="97f44-116">Weitere Informationen finden Sie unter [Exportieren von Inhalts Suchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="97f44-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="97f44-117">Wenn Sie mehr als 100K-Postfächer exportieren, müssen Sie die folgenden PowerShell verwenden, um die Exportergebnisse herunterzuladen:  [Exportieren von Ergebnissen aus mehr als 100K Postfächern](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="97f44-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>