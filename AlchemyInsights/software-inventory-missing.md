---
title: Fehlender oder ungenauer Softwarebestand
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658051"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="d184e-102">Fehlender oder ungenauer Softwarebestand</span><span class="sxs-lookup"><span data-stu-id="d184e-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="d184e-103">Der Softwarebestand in der Bedrohungs- und Sicherheitsrisikoverwaltung (TVM) ist eine Liste bekannter Software in Ihrer Organisation mit offiziellen CPEs (Common Platform Enumerations).</span><span class="sxs-lookup"><span data-stu-id="d184e-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="d184e-104">Für Softwareprodukte ohne offizielle CPE wurde keine Sicherheitsrisiken veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="d184e-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="d184e-105">Der Bestand umfasst auch Details wie den Namen des Anbieters, die Anzahl der Schwachstellen, Bedrohungen sowie die Anzahl der gefährdeten Geräte.</span><span class="sxs-lookup"><span data-stu-id="d184e-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="d184e-106">Softwareänderungen auf Geräten werden in der Regel innerhalb von zwei Stunden in Sicherheitsportalen widergespiegelt.</span><span class="sxs-lookup"><span data-stu-id="d184e-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="d184e-107">Es kann jedoch manchmal länger dauern.</span><span class="sxs-lookup"><span data-stu-id="d184e-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="d184e-108">Derzeit gibt es keine Möglichkeit, eine Synchronisierung zu erzwingen. Es handelt sich um eine kontinuierliche Bewertung.</span><span class="sxs-lookup"><span data-stu-id="d184e-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="d184e-109">Wenn Sie eine Softwareänderung vorgenommen haben und die Änderung nach 5 Stunden in TVM nicht präzise widergespiegelt wird, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="d184e-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="d184e-110">Überprüfen Sie den Abschnitt „Softwarenachweis“, um zu verstehen, wie die Software erkannt wurde.</span><span class="sxs-lookup"><span data-stu-id="d184e-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="d184e-111">Stellen Sie sicher, dass die Software unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="d184e-111">Make sure that the software is supported.</span></span> <span data-ttu-id="d184e-112">Software ist möglicherweise nur auf Geräteebene sichtbar, auch wenn sie aktuell nicht von der Bedrohungs- und Sicherheitsrisikoverwaltung unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="d184e-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="d184e-113">Es stehen jedoch nur eingeschränkte Daten zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d184e-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="d184e-114">Schritte, wie Sie Ungenauigkeiten im Portal melden können, finden Sie unter [Ungenauigkeit melden](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="d184e-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="d184e-115">**Hinweis**: Das Melden einer Ungenauigkeit über das MDE-Portal ist ein Einwegkanal für Techniker.</span><span class="sxs-lookup"><span data-stu-id="d184e-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="d184e-116">Wenn das Problem dringend ist, öffnen Sie ein Supportticket.</span><span class="sxs-lookup"><span data-stu-id="d184e-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="d184e-117">Weitere Informationen finden Sie unter [Softwarebestand – Bedrohungs- und Sicherheitsrisikoverwaltung](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="d184e-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>