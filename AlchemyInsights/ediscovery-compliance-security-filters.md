---
title: Während der Inhaltssuche/des Exports werden keine Ergebnisse zurückgegeben.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727222"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="59e9e-102">Während der Inhaltssuche/des Exports werden keine Ergebnisse zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59e9e-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="59e9e-103">Wenn Probleme mit den folgenden eDiscovery-Szenarien auftreten:</span><span class="sxs-lookup"><span data-stu-id="59e9e-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="59e9e-104">Inhaltssuche/-Export gibt keine Daten oder unerwartete Daten zurück</span><span class="sxs-lookup"><span data-stu-id="59e9e-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="59e9e-105">eDiscovery-Suche oder-Export schlägt fehl</span><span class="sxs-lookup"><span data-stu-id="59e9e-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="59e9e-106">Dies kann an bestimmten Sicherheitsfiltern für die Sicherheit liegen, die von einem bestimmten Administrator eingerichtet wurden und nicht allen Administratoren mitgeteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="59e9e-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="59e9e-107">Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die diese Probleme verursachen könnten:</span><span class="sxs-lookup"><span data-stu-id="59e9e-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="59e9e-108">Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="59e9e-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="59e9e-109">Führen Sie den folgenden Cmdlets aus:</span><span class="sxs-lookup"><span data-stu-id="59e9e-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="59e9e-110">Weitere Informationen zu Compliance-Sicherheitsfiltern finden Sie unter [Berechtigungs Filterung für die Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="59e9e-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
