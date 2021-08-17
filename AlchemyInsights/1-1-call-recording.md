---
title: 1:1-Anrufaufzeichnung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886138"
---
# <a name="11-call-recording"></a>1:1-Anrufaufzeichnung

Wenn die Schaltfläche **"Aufzeichnung starten"** in einem 1:1-Anruf ausgegraut ist, müssen Sie die Richtlinieneinstellungen für den betroffenen Benutzer ändern. Um die Richtlinieneinstellung zu überprüfen, führen Sie die Diagnose für den betroffenen Benutzer aus, indem Sie **Diag: Teams 1:1-Anrufaufzeichnung** oben eingeben.     

Ab dem 31. Mai 2021 werden wir eine neue Teams Anrufrichtlinie *AllowCloudRecordingForCalls* erzwingen. Vor dieser Änderung wird die Aufzeichnung von 1:1-Anrufen durch die *Besprechungsrichtlinie "AllowCloudRecording* Teams" gesteuert. Diese Änderung ist im Nachrichtencenterbeitrag dokumentiert: [(Aktualisiert) 1:1 Einführung in die Richtlinie für die Anrufaufzeichnung.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   Die Anrufrichtlinienoption ist standardmäßig auf **$False** festgelegt. Wenn Sie die Aufzeichnung von 1:1-Anrufen für alle Benutzer blockieren möchten, müssen Sie keine Maßnahmen ergreifen.  

Um die Anrufaufzeichnung für alle Benutzer in 1:1-Anrufen zu aktivieren, verwenden [Sie Teams PowerShell,](https://docs.microsoft.com/microsoftteams/teams-powershell-install) um das folgende Cmdlet auszuführen: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativ können Sie eine neue Richtlinie erstellen und **"-AllowCloudRecordingForCalls"** auf **$true** festlegen und diese Richtlinie Ihren Benutzern zuweisen. 

Weitere Informationen finden Sie unter ["1:1 Richtliniensteuerungen für die Aufzeichnung von Anrufen" (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
