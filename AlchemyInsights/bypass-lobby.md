---
title: Umgehungs Lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626347"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="6782e-102">Steuern der Lobby Einstellungen und Grad der Teilnahme</span><span class="sxs-lookup"><span data-stu-id="6782e-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="6782e-103">Wenn Sie möchten, dass jeder, einschließlich Einwahl, externen und anonymen Benutzern, die Lobby in Microsoft Teams umgehen kann, können Sie dies mithilfe von PowerShell tun.</span><span class="sxs-lookup"><span data-stu-id="6782e-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="6782e-104">Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation:</span><span class="sxs-lookup"><span data-stu-id="6782e-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="6782e-105">Dieses Cmdlet erfordert derzeit die Verwendung Skype for Business PowerShell-Moduls.</span><span class="sxs-lookup"><span data-stu-id="6782e-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="6782e-106">Informationen zum Einrichten der Verwendung dieses Cmdlets finden Sie unter [Managing Policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="6782e-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="6782e-107">Sie können eine neue Richtlinie einrichten, die Sie dann auf Benutzer anwenden müssen.</span><span class="sxs-lookup"><span data-stu-id="6782e-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="6782e-108">Wenn Sie die globale Richtlinie ändern, wird Sie automatisch auf Benutzer angewendet.</span><span class="sxs-lookup"><span data-stu-id="6782e-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="6782e-109">Bei jeder Richtlinienänderung müssen Sie mindestens 4 Stunden warten, bis die Richtlinien wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="6782e-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="6782e-110">Lesen Sie unbedingt die nachfolgende Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.</span><span class="sxs-lookup"><span data-stu-id="6782e-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="6782e-111">Grundlegendes zu Teams Besprechung Lobby Richtlinien Kontrollen</span><span class="sxs-lookup"><span data-stu-id="6782e-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="6782e-112">[Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.</span><span class="sxs-lookup"><span data-stu-id="6782e-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="6782e-113">[Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.</span><span class="sxs-lookup"><span data-stu-id="6782e-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="6782e-114">[Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .</span><span class="sxs-lookup"><span data-stu-id="6782e-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="6782e-115">[Organisatoren erlauben, Lobby Einstellungen außer Kraft zu setzen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**), ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator festgelegt hat, um Benutzer **automatisch** zuzulassen und **Einwahl Benutzern die Umgehung der Lobby zu ermöglichen** , wenn Sie eine neue Besprechung planen.</span><span class="sxs-lookup"><span data-stu-id="6782e-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="6782e-116">**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen.</span><span class="sxs-lookup"><span data-stu-id="6782e-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
