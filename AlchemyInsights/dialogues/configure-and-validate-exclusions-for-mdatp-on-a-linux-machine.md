---
title: Konfigurieren und Überprüfen von Ausschlüssen für MDATP auf einem Linux-Computer
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568615"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="5a922-102">Konfigurieren und Überprüfen von Ausschlüssen für MDATP auf einem Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="5a922-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="5a922-103">Sie können bestimmte Dateien, Ordner, Prozesse und prozessge öffnende Dateien aus MDATP-Scans ausschließen.</span><span class="sxs-lookup"><span data-stu-id="5a922-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="5a922-104">Ausschlüsse verhindern eine falsche Erkennung von Software und Dateien, die eindeutig oder an Ihre Organisation angepasst sind.</span><span class="sxs-lookup"><span data-stu-id="5a922-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="5a922-105">Ausschlüsse helfen auch bei der Verringerung von Leistungsproblemen, die durch MDATP verursacht werden.</span><span class="sxs-lookup"><span data-stu-id="5a922-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="5a922-106">Weitere Informationen finden Sie unter [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="5a922-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5a922-107">Die in diesem Artikel beschriebenen Ausschlüsse gelten nicht für andere Funktionen von MDATP für Linux, einschließlich Endpunkterkennung und -reaktion (EDR).</span><span class="sxs-lookup"><span data-stu-id="5a922-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="5a922-108">Dateien, die Sie mithilfe der in diesem Artikel beschriebenen Methoden ausschließen, können weiterhin EDR-Warnungen und andere Erkennungsfunktionen auslösen.</span><span class="sxs-lookup"><span data-stu-id="5a922-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
