---
title: Inhaltssuche keine Ergebnisse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800346"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="ac916-102">Keine Ergebnisse aus der Inhaltssuche/Exporte</span><span class="sxs-lookup"><span data-stu-id="ac916-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="ac916-103">Probleme bei der Inhaltssuche/Exporte, die keine Daten zurückgeben, können an einem bestimmten Compliance-Sicherheits Filter liegen, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert.</span><span class="sxs-lookup"><span data-stu-id="ac916-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="ac916-104">Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die dies möglicherweise verursachen:</span><span class="sxs-lookup"><span data-stu-id="ac916-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="ac916-105">Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="ac916-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ac916-106">Führen Sie den folgenden Cmdlets aus:</span><span class="sxs-lookup"><span data-stu-id="ac916-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="ac916-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="ac916-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="ac916-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="ac916-108">Get-ComplianceSecurityFilter -Organization $org</span></span>