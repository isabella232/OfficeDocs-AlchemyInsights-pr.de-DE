---
title: 1:1 Anrufaufzeichnung
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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702089"
---
# <a name="11-call-recording"></a>1:1 Anrufaufzeichnung

Wenn die **Schaltfläche Aufzeichnung** starten in einem 1:1-Anruf ausgegraut ist, müssen Sie die Richtlinieneinstellungen für den betroffenen Benutzer ändern. Um die Richtlinieneinstellung zu überprüfen, führen Sie die Diagnose für den betroffenen Benutzer aus, indem Sie **Diag: Teams 1:1 Anrufaufzeichnung oben** eingeben.     

Ab dem 31. Mai 2021 wird mit der Erzwingung einer neuen Teams-Anrufrichtlinie *AllowCloudRecordingForCalls gestartet.* Vor dieser Änderung wird die 1:1-Anrufaufzeichnung durch die *AllowCloudRecording-Teams* gesteuert. Diese Änderung wird im Beitrag Message Center dokumentiert: [(Aktualisiert) 1:1 Einführung](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)in die Richtlinie zur Anrufaufzeichnung.  

*AllowCloudRecordingForCalls*   Die Option zum Aufrufen der Richtlinie **ist standardmäßig auf $False** festgelegt. Wenn Sie es vorziehen, alle Benutzer an der Aufzeichnung von 1:1-Anrufen zu blockieren, müssen Sie keine Aktion ergreifen.  

Zum Aktivieren der Anrufaufzeichnung für alle Benutzer in 1:1-Anrufen verwenden Sie [Teams PowerShell](/microsoftteams/teams-powershell-install) zum Ausführen des folgenden Cmdlets: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativ können Sie eine neue Richtlinie erstellen und **-AllowCloudRecordingForCalls** so festlegen, **dass $true** benutzer zugewiesen werden. 

Weitere Informationen finden Sie unter [1:1 Anrufaufzeichnungsrichtliniensteuerelemente sind (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
