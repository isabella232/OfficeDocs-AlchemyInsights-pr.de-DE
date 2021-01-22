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
# <a name="turn-on-ndi-technology"></a>Aktivieren der NDI-Technologie

Für die NDI-Technologie müssen zwei Schritte für einen Benutzer aktiviert werden:

1. Der Mandantenadministrator muss die Eigenschaft "AllowNDIStreaming" in "CsTeamsMeetingPolicy" aktivieren.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nachdem diese Änderung aufgefüllt wurde, muss der Endbenutzer die NDI®Technologie für seinen bestimmten Client über einstellungen **> aktivieren.**

Weitere Informationen finden Sie unter [Verwenden der NDI-Technologie in Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
