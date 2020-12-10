---
title: 'Problembehandlung bei Voicemail '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608005"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="d0a2e-102">Problembehandlung bei Voicemail</span><span class="sxs-lookup"><span data-stu-id="d0a2e-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="d0a2e-103">Stellen Sie sicher, dass das Feature busy on Busy beabsichtigt ist.</span><span class="sxs-lookup"><span data-stu-id="d0a2e-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="d0a2e-104">Wenn dieses Feature für diesen Benutzer nicht erforderlich ist:</span><span class="sxs-lookup"><span data-stu-id="d0a2e-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="d0a2e-105">Wechseln Sie zu [Teams Admin Center](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="d0a2e-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="d0a2e-106">Navigieren Sie auf der linken Seite in Richtlinien für **VoIP**  >  -**Anrufe**  >  **Verwalten von Richtlinien** für die **Anrufrichtlinie**.</span><span class="sxs-lookup"><span data-stu-id="d0a2e-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="d0a2e-107">Wählen Sie **Benutzer verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="d0a2e-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="d0a2e-108">Suchen Sie nach dem Benutzer, und ändern Sie die Anrufrichtlinie in eine, die **beschäftigt in beschäftigt ist, ist verfügbar, wenn in einem Aufruf** **von Off**.</span><span class="sxs-lookup"><span data-stu-id="d0a2e-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="d0a2e-109">Klicken Sie auf **Anwenden**.</span><span class="sxs-lookup"><span data-stu-id="d0a2e-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="d0a2e-110">Änderungen an Richtlinien können bis zu 24 Stunden dauern, bis Sie repliziert werden.</span><span class="sxs-lookup"><span data-stu-id="d0a2e-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="d0a2e-111">Weitere Informationen zu diesem Feature finden Sie unter: [busy on Busy steht während eines Anrufs zur Verfügung](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="d0a2e-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
