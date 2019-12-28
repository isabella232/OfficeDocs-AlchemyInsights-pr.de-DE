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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889081"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="e5f05-102">Steuern von Lobby Einstellungen und Grad der Teilnahme an Teams</span><span class="sxs-lookup"><span data-stu-id="e5f05-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="e5f05-103">Wenn Sie möchten, dass jeder, einschließlich Einwahl, externen und anonymen Benutzern, **die Lobby umgehen**kann, verwenden Sie PowerShell, um diese Aufgabe auszuführen.</span><span class="sxs-lookup"><span data-stu-id="e5f05-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="e5f05-104">Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="e5f05-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="e5f05-105">Dieses Cmdlet erfordert derzeit die Verwendung Skype for Business PowerShell-Moduls.</span><span class="sxs-lookup"><span data-stu-id="e5f05-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="e5f05-106">Informationen zum Einrichten für die Verwendung dieses Cmdlets finden Sie unter [Managing Policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="e5f05-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="e5f05-107">Nachdem Sie eine Richtlinie eingerichtet haben, müssen Sie Sie auf die Benutzer anwenden. oder wenn Sie die globale Richtlinie geändert haben, wird Sie automatisch auf Benutzer angewendet.</span><span class="sxs-lookup"><span data-stu-id="e5f05-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="e5f05-108">Bei jeder Richtlinienänderung müssen Sie mindestens **4 Stunden bis zu 24 Stunden** warten, bis die Richtlinien wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="e5f05-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="e5f05-109">Lesen Sie unbedingt die nachfolgende Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.</span><span class="sxs-lookup"><span data-stu-id="e5f05-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="e5f05-110">Grundlegendes zu Teams Besprechung Lobby Richtlinien Kontrollen</span><span class="sxs-lookup"><span data-stu-id="e5f05-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="e5f05-111">Mit diesen Einstellungen wird gesteuert, welche Besprechungsteilnehmer in der Lobby warten, bevor Sie zur Besprechung zugelassen werden, und die Teilnahmestufe, die Sie in einer Besprechung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="e5f05-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="e5f05-112">Sie können PowerShell verwenden, um Besprechungsrichtlinien Einstellungen zu aktualisieren, die noch nicht implementiert wurden (mit der Bezeichnung "Coming Soon") im Teamadministrator Center.</span><span class="sxs-lookup"><span data-stu-id="e5f05-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="e5f05-113">Im folgenden finden Sie ein Beispiel für ein PowerShell-Cmdlet, das es allen Benutzern ermöglicht, die Lobby zu umgehen.</span><span class="sxs-lookup"><span data-stu-id="e5f05-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="e5f05-114">[Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.</span><span class="sxs-lookup"><span data-stu-id="e5f05-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e5f05-115">[Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.</span><span class="sxs-lookup"><span data-stu-id="e5f05-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e5f05-116">[Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .</span><span class="sxs-lookup"><span data-stu-id="e5f05-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e5f05-117">[Organisatoren erlauben, Lobby Einstellungen außer Kraft zu setzen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**), ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator festgelegt hat, um Benutzer **automatisch** zuzulassen und **Einwahl Benutzern die Umgehung der Lobby zu ermöglichen** , wenn Sie eine neue Besprechung planen.</span><span class="sxs-lookup"><span data-stu-id="e5f05-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e5f05-118">**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen.</span><span class="sxs-lookup"><span data-stu-id="e5f05-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
