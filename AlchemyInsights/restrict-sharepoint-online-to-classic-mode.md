---
title: SharePoint Online auf den klassischen Modus beschränken
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752067"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="b6f74-102">SharePoint Online auf den klassischen Modus beschränken</span><span class="sxs-lookup"><span data-stu-id="b6f74-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="b6f74-103">Einige Organisationen benötigen weiterhin die klassische Modus-Erfahrung.</span><span class="sxs-lookup"><span data-stu-id="b6f74-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="b6f74-104">Es gibt zwar keine Pläne, den klassischen Modus auf granularer Ebene zu entfernen, es ist jedoch nicht mehr möglich, eine gesamte Organisation (einen Mandanten) auf den klassischen Modus für Listen und Bibliotheken zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="b6f74-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="b6f74-105">Der Administrator verfügt über die folgenden Optionen zum Verwalten einzelner Listen und Bibliotheken im klassischen Modus mithilfe von granularen Opt-out-Switches, die auf den folgenden Ebenen bereitgestellt werden:</span><span class="sxs-lookup"><span data-stu-id="b6f74-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="b6f74-106">Websitesammlung</span><span class="sxs-lookup"><span data-stu-id="b6f74-106">site collection</span></span>
- <span data-ttu-id="b6f74-107">Website</span><span class="sxs-lookup"><span data-stu-id="b6f74-107">site</span></span>
- <span data-ttu-id="b6f74-108">Liste</span><span class="sxs-lookup"><span data-stu-id="b6f74-108">list</span></span>
- <span data-ttu-id="b6f74-109">Bibliothek</span><span class="sxs-lookup"><span data-stu-id="b6f74-109">library</span></span>

<span data-ttu-id="b6f74-110">Außerdem werden Listen, die bestimmte Features und Anpassungen verwenden, die nicht von modern unterstützt werden, weiterhin automatisch in den klassischen Modus umgeschaltet.</span><span class="sxs-lookup"><span data-stu-id="b6f74-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="b6f74-111">Ab dem 1. April 2019 wird der Vorgang zum Deaktivieren der Mandantenebene aus modernen Listen und Bibliotheken gestartet und wird bis zum 31. Mai 2019 fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="b6f74-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="b6f74-112">Die Listen und Bibliotheken, die sich im klassischen Modus infolge eines Mandanten Abmeldens befinden, werden automatisch auf modern verschoben.</span><span class="sxs-lookup"><span data-stu-id="b6f74-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="b6f74-113">Wenn Sie den klassischen Modus benötigen, lesen Sie hier [Weitere Informationen und](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) hier finden Sie die PNP-PowerShell-Anweisung, in der Optionen und Tools beschrieben [werden, die](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) Sie heute verwenden können, um die klassische Benutzeroberfläche zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="b6f74-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
