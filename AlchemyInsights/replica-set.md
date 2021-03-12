---
title: Replikatsatz
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716271"
---
# <a name="replica-set"></a><span data-ttu-id="21944-102">Replikatsatz</span><span class="sxs-lookup"><span data-stu-id="21944-102">Replica set</span></span>

<span data-ttu-id="21944-103">AADDS wird auch als verwaltete Domäne bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="21944-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="21944-104">Es handelt sich tatsächlich um zwei Domänencontroller, die vom Back-End ausgeführt und verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="21944-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="21944-105">Die beiden DCs umfassen einen Haupt-DC und einen Replikations-DC.</span><span class="sxs-lookup"><span data-stu-id="21944-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="21944-106">Sicherungen in AADDS (verwaltete Domäne) sind ein automatisierter Prozess, der von der Azure-Plattform verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="21944-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="21944-107">Im Falle eines Problems mit Ihrer verwalteten Domäne kann die Azure-Unterstützung Ihnen bei der Wiederherstellung aus der Sicherung helfen.</span><span class="sxs-lookup"><span data-stu-id="21944-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="21944-108">Sie erstellen jeden Replikatsatz in einem virtuellen Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="21944-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="21944-109">Jedes virtuelle Netzwerk muss mit jedem anderen virtuellen Netzwerk, das den Replikatsatz einer verwalteten Domäne hostet, peered werden.</span><span class="sxs-lookup"><span data-stu-id="21944-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="21944-110">Diese Konfiguration erstellt eine Gitternetzwerktopologie, die die Verzeichnisreplikation unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21944-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="21944-111">Ein virtuelles Netzwerk kann mehrere Replikatsätze unterstützen, sofern sich jeder Replikatsatz in einem anderen virtuellen Subnetz befindet.</span><span class="sxs-lookup"><span data-stu-id="21944-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="21944-112">Weitere Informationen zum Replikatsatz finden Sie unter [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="21944-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
