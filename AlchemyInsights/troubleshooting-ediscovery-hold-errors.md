---
title: Beheben von Fehlern bei der eDiscovery-Aufbewahrung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583754"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="e7349-102">Beheben von Fehlern bei der eDiscovery-Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="e7349-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="e7349-103">Gibt es Probleme bei der eDiscovery-Aufbewahrung?</span><span class="sxs-lookup"><span data-stu-id="e7349-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="e7349-104">Hier finden Sie einige bewährte Methoden, die Sie berücksichtigen sollten:</span><span class="sxs-lookup"><span data-stu-id="e7349-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="e7349-105">Überprüfen Sie den Verteilungsstatus der Aufbewahrung.</span><span class="sxs-lookup"><span data-stu-id="e7349-105">Check the hold distribution status.</span></span>  <span data-ttu-id="e7349-106">Wenn der Status auf **Ein (Ausstehend)** oder **Aus (Ausstehend)** festgelegt ist, warten Sie, bis die Aufbewahrungsverteilung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="e7349-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="e7349-107">Führen Sie eDiscovery-Aufbewahrungsaktualisierungen in einer einzelnen Massenanforderung zusammen, statt die Richtlinie für jede Transaktion einzeln zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="e7349-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="e7349-108">Führen Sie „Set-CaseHoldPolicy <policyname> -RetryDistribution“ in der Security und Compliance Center-PowerShell aus.</span><span class="sxs-lookup"><span data-stu-id="e7349-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="e7349-109">Details finden Sie unter [Herstellen einer Verbindung mit der Security und Compliance Center-PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="e7349-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="e7349-110">Schritte zum Überprüfen dieser Einstellungen und weitere bewährte Methoden für die Verringerung und Behebung von Problemen bei der eDiscovery-Aufbewahrung finden Sie unter [Beheben von Fehlern bei der eDiscovery-Aufbewahrung](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="e7349-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="e7349-111">Informationen zur Problembehandlung bei anderen häufigen eDiscovery-Problemen finden Sie unter [Untersuchung, Problembehandlung und Lösung häufiger eDiscovery-Probleme](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="e7349-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
