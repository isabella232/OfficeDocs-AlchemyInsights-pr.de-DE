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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516778"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="45f0b-102">Keine Ergebnisse aus der Inhaltssuche/Exporte</span><span class="sxs-lookup"><span data-stu-id="45f0b-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="45f0b-103">Probleme bei der Inhaltssuche/Exporte, die keine Daten zurückgeben, können an einem bestimmten Compliance-Sicherheits Filter liegen, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert.</span><span class="sxs-lookup"><span data-stu-id="45f0b-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="45f0b-104">Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die dies möglicherweise verursachen:</span><span class="sxs-lookup"><span data-stu-id="45f0b-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="45f0b-105">Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="45f0b-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="45f0b-106">Führen Sie den folgenden Cmdlets aus:</span><span class="sxs-lookup"><span data-stu-id="45f0b-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="45f0b-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="45f0b-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="45f0b-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="45f0b-108">Get-ComplianceSecurityFilter -Organization $org</span></span>