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
# <a name="11-call-recording"></a><span data-ttu-id="ded7b-102">1:1 Anrufaufzeichnung</span><span class="sxs-lookup"><span data-stu-id="ded7b-102">1:1 call recording</span></span>

<span data-ttu-id="ded7b-103">Wenn die **Schaltfläche Aufzeichnung** starten in einem 1:1-Anruf ausgegraut ist, müssen Sie die Richtlinieneinstellungen für den betroffenen Benutzer ändern.</span><span class="sxs-lookup"><span data-stu-id="ded7b-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="ded7b-104">Um die Richtlinieneinstellung zu überprüfen, führen Sie die Diagnose für den betroffenen Benutzer aus, indem Sie **Diag: Teams 1:1 Anrufaufzeichnung oben** eingeben.</span><span class="sxs-lookup"><span data-stu-id="ded7b-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="ded7b-105">Ab dem 31. Mai 2021 wird mit der Erzwingung einer neuen Teams-Anrufrichtlinie *AllowCloudRecordingForCalls gestartet.*</span><span class="sxs-lookup"><span data-stu-id="ded7b-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="ded7b-106">Vor dieser Änderung wird die 1:1-Anrufaufzeichnung durch die *AllowCloudRecording-Teams* gesteuert.</span><span class="sxs-lookup"><span data-stu-id="ded7b-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="ded7b-107">Diese Änderung wird im Beitrag Message Center dokumentiert: [(Aktualisiert) 1:1 Einführung](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)in die Richtlinie zur Anrufaufzeichnung.</span><span class="sxs-lookup"><span data-stu-id="ded7b-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="ded7b-108">*AllowCloudRecordingForCalls*   Die Option zum Aufrufen der Richtlinie **ist standardmäßig auf $False** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ded7b-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="ded7b-109">Wenn Sie es vorziehen, alle Benutzer an der Aufzeichnung von 1:1-Anrufen zu blockieren, müssen Sie keine Aktion ergreifen.</span><span class="sxs-lookup"><span data-stu-id="ded7b-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="ded7b-110">Zum Aktivieren der Anrufaufzeichnung für alle Benutzer in 1:1-Anrufen verwenden Sie [Teams PowerShell](/microsoftteams/teams-powershell-install) zum Ausführen des folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="ded7b-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="ded7b-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="ded7b-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="ded7b-112">Alternativ können Sie eine neue Richtlinie erstellen und **-AllowCloudRecordingForCalls** so festlegen, **dass $true** benutzer zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="ded7b-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="ded7b-113">Weitere Informationen finden Sie unter [1:1 Anrufaufzeichnungsrichtliniensteuerelemente sind (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="ded7b-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
