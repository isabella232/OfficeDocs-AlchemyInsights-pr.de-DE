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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733848"
---
# <a name="11-call-recording"></a>1:1 Anrufaufzeichnung

Administratoren müssen jetzt Maßnahmen ergreifen, damit Benutzer weiterhin 1:1-Anrufe aufzeichnen können.
 
Ab dem 12. April 2021 wird mit der Erzwingung einer neuen Option für Die Anrufrichtlinie von Teams *allowCloudRecordingForCalls gestartet.* 

Derzeit werden 1:1-Anrufaufzeichnungsfunktionen durch die *Option AllowCloudRecording* in Teams-Besprechungsrichtlinien gesteuert. Wenn Ihre Benutzer Teams-Besprechungen aufzeichnen dürfen, können sie auch 1:1-Anrufe aufzeichnen.

Wenn Sie es vorziehen, alle Benutzer an der Aufzeichnung von 1:1-Anrufen zu blockieren, müssen Sie keine Aktion ergreifen. *Die Option allowCloudRecordingForCalls-Anrufrichtlinie* wird standardmäßig $False aktiviert.

Diese Änderung ist in der folgenden Message Center Post dokumentiert: [(Aktualisiert) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Einführung in die Anrufaufzeichnungsrichtlinie Zum Festlegen der Option "Teams-Anrufrichtlinie" müssen Sie [Teams PowerShell verwenden.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**So aktivieren Sie die Anrufaufzeichnung in 1:1-Anrufen:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**So deaktivieren Sie die Anrufaufzeichnung in 1:1-Anrufen:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

