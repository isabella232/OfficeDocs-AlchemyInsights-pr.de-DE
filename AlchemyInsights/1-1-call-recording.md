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
# <a name="11-call-recording"></a><span data-ttu-id="1a8b4-102">1:1 Anrufaufzeichnung</span><span class="sxs-lookup"><span data-stu-id="1a8b4-102">1:1 call recording</span></span>

<span data-ttu-id="1a8b4-103">Administratoren müssen jetzt Maßnahmen ergreifen, damit Benutzer weiterhin 1:1-Anrufe aufzeichnen können.</span><span class="sxs-lookup"><span data-stu-id="1a8b4-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="1a8b4-104">Ab dem 12. April 2021 wird mit der Erzwingung einer neuen Option für Die Anrufrichtlinie von Teams *allowCloudRecordingForCalls gestartet.*</span><span class="sxs-lookup"><span data-stu-id="1a8b4-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="1a8b4-105">Derzeit werden 1:1-Anrufaufzeichnungsfunktionen durch die *Option AllowCloudRecording* in Teams-Besprechungsrichtlinien gesteuert.</span><span class="sxs-lookup"><span data-stu-id="1a8b4-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="1a8b4-106">Wenn Ihre Benutzer Teams-Besprechungen aufzeichnen dürfen, können sie auch 1:1-Anrufe aufzeichnen.</span><span class="sxs-lookup"><span data-stu-id="1a8b4-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="1a8b4-107">Wenn Sie es vorziehen, alle Benutzer an der Aufzeichnung von 1:1-Anrufen zu blockieren, müssen Sie keine Aktion ergreifen.</span><span class="sxs-lookup"><span data-stu-id="1a8b4-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="1a8b4-108">*Die Option allowCloudRecordingForCalls-Anrufrichtlinie* wird standardmäßig $False aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1a8b4-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="1a8b4-109">Diese Änderung ist in der folgenden Message Center Post dokumentiert: [(Aktualisiert) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Einführung in die Anrufaufzeichnungsrichtlinie Zum Festlegen der Option "Teams-Anrufrichtlinie" müssen Sie [Teams PowerShell verwenden.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="1a8b4-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="1a8b4-110">**So aktivieren Sie die Anrufaufzeichnung in 1:1-Anrufen:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="1a8b4-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="1a8b4-111">**So deaktivieren Sie die Anrufaufzeichnung in 1:1-Anrufen:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="1a8b4-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

