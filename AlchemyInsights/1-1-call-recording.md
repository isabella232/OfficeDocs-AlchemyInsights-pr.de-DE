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
ms.openlocfilehash: befb89c28396be3dc60d9d812a0c6aced69bea3c1c48d88a4ab81a34d6c259b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918990"
---
# <a name="11-call-recording"></a>1:1-Anrufaufzeichnung

Wenn die Schaltfläche **"Aufzeichnung starten"** in einem 1:1-Anruf ausgegraut ist, müssen Sie die Richtlinieneinstellungen für den betroffenen Benutzer ändern. Um die Richtlinieneinstellung zu überprüfen, führen Sie die Diagnose für den betroffenen Benutzer aus, indem Sie **Diag: Teams 1:1-Anrufaufzeichnung** oben eingeben.     

Ab dem 31. Mai 2021 wird eine neue Teams Anrufrichtlinie *AllowCloudRecordingForCalls* erzwungen. Vor dieser Änderung wird die Aufzeichnung von 1:1-Anrufen durch die *Besprechungsrichtlinie "AllowCloudRecording* Teams" gesteuert. Diese Änderung ist im Nachrichtencenterbeitrag dokumentiert: [(Aktualisiert) 1:1 Einführung in die Richtlinie für die Anrufaufzeichnung.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   Die Anrufrichtlinienoption ist standardmäßig auf **$False** festgelegt. Wenn Sie die Aufzeichnung von 1:1-Anrufen für alle Benutzer blockieren möchten, müssen Sie keine Maßnahmen ergreifen.  

Verwenden Sie [Teams PowerShell,](/microsoftteams/teams-powershell-install) um die Anrufaufzeichnung für alle Benutzer in 1:1-Anrufen zu aktivieren, um das folgende Cmdlet auszuführen: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativ können Sie eine neue Richtlinie erstellen und **"-AllowCloudRecordingForCalls"** auf **$true** festlegen und diese Richtlinie Ihren Benutzern zuweisen. 

Weitere Informationen finden Sie unter ["1:1 Richtliniensteuerungen für die Aufzeichnung von Anrufen" (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
