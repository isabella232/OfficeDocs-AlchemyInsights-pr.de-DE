---
title: Einschränken von SharePoint Online auf den klassischen Modus
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32422174"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="d3d0a-102">Einschränken von SharePoint Online auf den klassischen Modus</span><span class="sxs-lookup"><span data-stu-id="d3d0a-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="d3d0a-103">Einige Organisationen benötigen weiterhin den klassischen Modus.</span><span class="sxs-lookup"><span data-stu-id="d3d0a-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="d3d0a-104">Es gibt zwar keine Pläne, den klassischen Modus auf einer granularen Ebene zu entfernen, ab dem 1. April 2019 ist es jedoch nicht mehr möglich, eine gesamte Organisation (Mandant) für Listen und Bibliotheken auf den klassischen Modus zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="d3d0a-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="d3d0a-105">Der Administrator hat die folgenden Optionen zum Verwalten einzelner Listen und Bibliotheken im klassischen Modus mit detaillierten Opt-out-Switches, die wir auf den folgenden Ebenen bereitstellen:</span><span class="sxs-lookup"><span data-stu-id="d3d0a-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="d3d0a-106">Websitesammlung</span><span class="sxs-lookup"><span data-stu-id="d3d0a-106">site collection</span></span>
- <span data-ttu-id="d3d0a-107">Website</span><span class="sxs-lookup"><span data-stu-id="d3d0a-107">site</span></span>
- <span data-ttu-id="d3d0a-108">Liste</span><span class="sxs-lookup"><span data-stu-id="d3d0a-108">list</span></span>
- <span data-ttu-id="d3d0a-109">Bibliothek</span><span class="sxs-lookup"><span data-stu-id="d3d0a-109">library</span></span>

<span data-ttu-id="d3d0a-110">Darüber hinaus werden Listen, die bestimmte Features und Anpassungen verwenden, die von modern nicht unterstützt werden, weiterhin automatisch in den klassischen Modus gewechselt.</span><span class="sxs-lookup"><span data-stu-id="d3d0a-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="d3d0a-111">Nach dem 1. April werden Listen und Bibliotheken, die als Ergebnis der Mandanten Aktivierung im klassischen Modus ausgeführt werden, automatisch auf Website-und Listenebene verwaltet.</span><span class="sxs-lookup"><span data-stu-id="d3d0a-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="d3d0a-112">Wenn Sie den klassischen Modus benötigen, finden Sie weitere Informationen hier und PnP PowerShell-Anweisung hier, die Optionen und Tools beschreibt, die Sie heute verwenden können, um die Deaktivierung der Mandantenebene am 1. April vorzubereiten.</span><span class="sxs-lookup"><span data-stu-id="d3d0a-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
