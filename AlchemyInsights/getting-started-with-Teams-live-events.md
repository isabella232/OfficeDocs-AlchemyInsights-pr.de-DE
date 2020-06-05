---
title: Erste Schritte mit Live-Veranstaltungen in Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 6ddb1e74d6c7217303da4f21a3bd71cdab3eb871
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563617"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="3a503-102">Erste Schritte mit Live-Veranstaltungen in Teams</span><span class="sxs-lookup"><span data-stu-id="3a503-102">Getting started with Teams live events</span></span>

<span data-ttu-id="3a503-103">Live-Ereignisse in Microsoft Teams sind eine Erweiterung von Teambesprechungen, die es Ihnen ermöglichen, Veranstaltungen bzw. Ereignisse zu planen und zu erstellen, die an ein zahlenmäßig großes Online-Publikum übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="3a503-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="3a503-104">Zum Erstellen eines Live-Ereignisses benötigen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="3a503-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="3a503-105">Vergewissern Sie sich zunächst, dass Teams-Liveereignisse [in Ihrem Land und Ihrer Region verfügbar sind](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability). Liveereignisse werden in einigen Ländern noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a503-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="3a503-106">Wenn Sie Lizenzen zugewiesen und Richtlinien festgelegt haben, aber immer noch kein Teams-Liveereignis erstellen können, befinden Sie sich wahrscheinlich in einem Land oder einer Region, in dem bzw. der Liveereignisse noch nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="3a503-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="3a503-107">Eine [Lizenz für Office 365 Enterprise E1, E3 oder E5 oder eine Lizenz für Office 365 A3 oder A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="3a503-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="3a503-108">**Hinweis**: Aufgrund der aktuell gestiegenen Nutzung von Teams, kann es möglicherweise bis zu 24 Stunden dauern, bis ein Benutzer, dem Sie eine Teams-Lizenz zugewiesen haben, vollständig eingerichtet ist.</span><span class="sxs-lookup"><span data-stu-id="3a503-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="3a503-109">Bis zu diesem Zeitpunkt sind Sie nicht in der Lage, diesen Benutzern Teams-Richtlinien zuzuweisen, und diese haben möglicherweise keinen Zugriff auf einige Teams-Features wie Anrufe und Audiokonferenzen.</span><span class="sxs-lookup"><span data-stu-id="3a503-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="3a503-110">Die Berechtigung zum [Erstellen von Live-Ereignissen im Microsoft Teams Admin Center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="3a503-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="3a503-111">Die Berechtigung zum [Erstellen von Live Ereignissen in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (für Ereignisse, die mit einer externen Broadcasting-App oder einem externen Gerät erstellt wurden).</span><span class="sxs-lookup"><span data-stu-id="3a503-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="3a503-112">Vollständige Teammitgliedschaft in der Organisation (darf kann kein Gast oder jemand von einer anderen Organisation sein)</span><span class="sxs-lookup"><span data-stu-id="3a503-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="3a503-113">Planung von privaten Besprechungen, Screensharing und IP-Videofreigabe – in der Team-Besprechungsrichtlinie aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3a503-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="3a503-114">[Bewährte Methoden](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) für Live-Ereignisse in Teams.</span><span class="sxs-lookup"><span data-stu-id="3a503-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="3a503-115">Weitere Informationen finden Sie unter [Erste Schritte mit Microsoft Teams Live-Ereignissen](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="3a503-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>