---
title: SharePoint Online auf den klassischen Modus beschränken
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751421"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="1962e-102">SharePoint Online auf den klassischen Modus beschränken</span><span class="sxs-lookup"><span data-stu-id="1962e-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="1962e-103">Einige Organisationen benötigen weiterhin die klassische Modus-Erfahrung.</span><span class="sxs-lookup"><span data-stu-id="1962e-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="1962e-104">Es gibt zwar keine Pläne, den klassischen Modus auf granularer Ebene zu entfernen, es ist jedoch nicht mehr möglich, eine gesamte Organisation (einen Mandanten) auf den klassischen Modus für Listen und Bibliotheken zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="1962e-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="1962e-105">Der Administrator verfügt über die folgenden Optionen zum Verwalten einzelner Listen und Bibliotheken im klassischen Modus mithilfe von granularen Opt-out-Switches, die auf den folgenden Ebenen bereitgestellt werden:</span><span class="sxs-lookup"><span data-stu-id="1962e-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="1962e-106">Websitesammlung</span><span class="sxs-lookup"><span data-stu-id="1962e-106">site collection</span></span>
- <span data-ttu-id="1962e-107">Website</span><span class="sxs-lookup"><span data-stu-id="1962e-107">site</span></span>
- <span data-ttu-id="1962e-108">Liste</span><span class="sxs-lookup"><span data-stu-id="1962e-108">list</span></span>
- <span data-ttu-id="1962e-109">Bibliothek</span><span class="sxs-lookup"><span data-stu-id="1962e-109">library</span></span>

<span data-ttu-id="1962e-110">Außerdem werden Listen, die bestimmte Features und Anpassungen verwenden, die nicht von modern unterstützt werden, weiterhin automatisch in den klassischen Modus umgeschaltet.</span><span class="sxs-lookup"><span data-stu-id="1962e-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="1962e-111">Ab dem 1. April 2019 wird der Vorgang zum Deaktivieren der Mandantenebene aus modernen Listen und Bibliotheken gestartet und wird bis zum 31. Mai 2019 fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="1962e-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="1962e-112">Die Listen und Bibliotheken, die sich im klassischen Modus infolge eines Mandanten Abmeldens befinden, werden automatisch auf modern verschoben.</span><span class="sxs-lookup"><span data-stu-id="1962e-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="1962e-113">Wenn Sie den klassischen Modus benötigen, lesen Sie hier [Weitere Informationen und](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) hier finden Sie die PNP-PowerShell-Anweisung, in der Optionen und Tools beschrieben [werden, die](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) Sie heute verwenden können, um die klassische Benutzeroberfläche zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="1962e-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
