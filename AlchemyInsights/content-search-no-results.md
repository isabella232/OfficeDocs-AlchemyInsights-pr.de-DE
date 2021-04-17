---
title: Inhaltssuche Keine Ergebnisse
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816847"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="94a31-102">Keine Ergebnisse aus inhaltssuche/export</span><span class="sxs-lookup"><span data-stu-id="94a31-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="94a31-103">Probleme mit der Inhaltssuche/-exporten, die keine Daten zurückgeben, können auf bestimmten Compliancesicherheitsfilter zurück, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert wurde.</span><span class="sxs-lookup"><span data-stu-id="94a31-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="94a31-104">Um dies zu beheben, überprüfen Sie, ob Kompatibilitätssicherheitsfilter enthalten sind, die dies verursachen können:</span><span class="sxs-lookup"><span data-stu-id="94a31-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="94a31-105">Herstellen einer Verbindung mit Security and Compliance Center Powershell</span><span class="sxs-lookup"><span data-stu-id="94a31-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="94a31-106">Führen Sie die folgenden Befehlslets aus:</span><span class="sxs-lookup"><span data-stu-id="94a31-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="94a31-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="94a31-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="94a31-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="94a31-108">Get-ComplianceSecurityFilter -Organization $org</span></span>