---
title: Aktivieren der NDI-Technologie
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917313"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="a9df3-102">Aktivieren der NDI-Technologie</span><span class="sxs-lookup"><span data-stu-id="a9df3-102">Turn on NDI technology</span></span>

<span data-ttu-id="a9df3-103">Für die NDI-Technologie müssen zwei Schritte für einen Benutzer aktiviert werden:</span><span class="sxs-lookup"><span data-stu-id="a9df3-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="a9df3-104">Der Mandantenadministrator muss die Eigenschaft "AllowNDIStreaming" in "CsTeamsMeetingPolicy" aktivieren.</span><span class="sxs-lookup"><span data-stu-id="a9df3-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="a9df3-105">Nachdem diese Änderung aufgefüllt wurde, muss der Endbenutzer die NDI®Technologie für seinen bestimmten Client über einstellungen **> aktivieren.**</span><span class="sxs-lookup"><span data-stu-id="a9df3-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="a9df3-106">Weitere Informationen finden Sie unter [Verwenden der NDI-Technologie in Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="a9df3-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
