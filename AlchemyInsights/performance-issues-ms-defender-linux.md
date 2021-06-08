---
title: Leistungsprobleme bei Microsoft Defender für Endpunkt unter Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783434"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="1b20d-102">Leistungsprobleme bei Microsoft Defender für Endpunkt unter Linux</span><span class="sxs-lookup"><span data-stu-id="1b20d-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="1b20d-103">Dieser Artikel führt Sie durch die Schritte zum Identifizieren von Leistungsproblemen bei Microsoft Defender für Endpunkt unter Linux.</span><span class="sxs-lookup"><span data-stu-id="1b20d-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="1b20d-104">Es ist wichtig zuerst zu überprüfen, ob das Problem mit der [aktuellsten Version](/microsoft-365/security/defender-endpoint/linux-whatsnew) behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="1b20d-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="1b20d-105">Informationen zum Starten Ihrer Untersuchung finden Sie unter [Behandeln von Leistungsproblemen bei Microsoft Defender für Endpunkt unter Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="1b20d-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="1b20d-106">Ausschlüsse</span><span class="sxs-lookup"><span data-stu-id="1b20d-106">Exclusions</span></span>

<span data-ttu-id="1b20d-107">Ausschlüsse können zur Entschärfung von Leistungsproblemen beitragen.</span><span class="sxs-lookup"><span data-stu-id="1b20d-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="1b20d-108">Überprüfen Sie Ihre Ausschlüsse, bevor Sie beginnen, damit zusätzliche Risiken bekannt und dokumentiert sind.</span><span class="sxs-lookup"><span data-stu-id="1b20d-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="1b20d-109">Weitere Informationen finden Sie unter [Konfigurieren und Überprüfen von Ausschlüssen für Microsoft Defender für Endpunkt unter Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="1b20d-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="1b20d-110">Wenn Sie mehrere Dateien und Ordner ausschließen möchten und diese sich alle am selben Bereitstellungspunkt befinden, könnte es einfacher sein, den Bereitstellungspunkt auszuschließen.</span><span class="sxs-lookup"><span data-stu-id="1b20d-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="1b20d-111">Beginnend mit der Februar-Version 101.22.80 können Sie einen gesamten Bereitstellungspunkt ausschließen.</span><span class="sxs-lookup"><span data-stu-id="1b20d-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="1b20d-112">Wenn z. B. "/mnt/backup" ein Bereitstellungspunkt ist, können Sie der Ausschlussliste "/mnt/backup" hinzufügen, indem Sie den folgenden Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="1b20d-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="1b20d-113">**Hinweis**: Durch das Hinzufügen von Ausschlüssen erhöht sich das Risiko, dass Schadsoftware nicht erkannt wird. Das Ausschließen sollte mit Bedacht eingesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="1b20d-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="1b20d-114">Benötigen Sie Hilfe?</span><span class="sxs-lookup"><span data-stu-id="1b20d-114">Need Help?</span></span>

<span data-ttu-id="1b20d-115">Sammeln Sie die Diagnosedaten, bevor Sie einen Supportfall öffnen, damit wir Ihnen so effizient wie möglich helfen können.</span><span class="sxs-lookup"><span data-stu-id="1b20d-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
