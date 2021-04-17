---
title: Umgehungslobby
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820033"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="7e92a-102">Steuern der Lobbyeinstellungen und des Grads der Teilnahme an Teams</span><span class="sxs-lookup"><span data-stu-id="7e92a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="7e92a-103">Wenn Sie allen Benutzern, einschließlich Einwahlbenutzern, externen und anonymen Benutzern, erlauben möchten, die Lobby zu **umgehen,** verwenden Sie PowerShell, um diese Aufgabe zu erledigen.</span><span class="sxs-lookup"><span data-stu-id="7e92a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="7e92a-104">Hier sehen Sie ein Beispiel für das Ändern der globalen Besprechungsrichtlinie für Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="7e92a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7e92a-105">Dieses Cmdlet erfordert derzeit die Verwendung des Skype for Business PowerShell-Moduls.</span><span class="sxs-lookup"><span data-stu-id="7e92a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7e92a-106">Informationen zur Einrichtung für die Verwendung dieses Cmdlets erhalten Sie unter [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="7e92a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7e92a-107">Nachdem Sie eine Richtlinie eingerichtet haben, müssen Sie sie auf Benutzer anwenden. oder, wenn Sie die globale Richtlinie geändert haben, gilt sie automatisch für Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7e92a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="7e92a-108">Für jede Richtlinienänderung müssen Sie mindestens 4 Stunden bis **zu 24** Stunden warten, bis die Richtlinien wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="7e92a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="7e92a-109">Lesen Sie unbedingt die unten aufgeführte Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.</span><span class="sxs-lookup"><span data-stu-id="7e92a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7e92a-110">Grundlegendes zu Richtliniensteuerelementen für Besprechungslobbys in Teams</span><span class="sxs-lookup"><span data-stu-id="7e92a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="7e92a-111">Diese Einstellungen steuern, welche Besprechungsteilnehmer in der Lobby warten, bevor sie zur Besprechung zugelassen werden, und welche Teilnehmer an einer Besprechung teilnehmen dürfen.</span><span class="sxs-lookup"><span data-stu-id="7e92a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7e92a-112">Sie können PowerShell verwenden, um Besprechungsrichtlinieneinstellungen zu aktualisieren, die noch nicht implementiert wurden (mit der Bezeichnung "bald verfügbar") im Teams Admin Center.</span><span class="sxs-lookup"><span data-stu-id="7e92a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="7e92a-113">Ein Beispiel für ein PowerShell-Cmdlet, mit dem alle Benutzer die Lobby umgehen können, finden Sie unten.</span><span class="sxs-lookup"><span data-stu-id="7e92a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="7e92a-114">[Die automatische Zulassung](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) von Personen ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis sie von einem authentifizierten Benutzer zugelassen werden.</span><span class="sxs-lookup"><span data-stu-id="7e92a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7e92a-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Das Starten einer Besprechung durch anonyme Personen ist eine Richtlinie pro Organisator, die steuert, ob anonyme Personen, einschließlich B2B- und Verbundbenutzer, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer aus der Organisation anwesend ist.</span><span class="sxs-lookup"><span data-stu-id="7e92a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7e92a-116">Zulassen, dass Einwahlbenutzer die Lobby [(](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) in Kürze **)** umgehen, ist eine Richtlinie pro Organisator, die steuert,  ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung Personen automatisch zulassen.</span><span class="sxs-lookup"><span data-stu-id="7e92a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7e92a-117">Organisatoren das Außerkraft setzen von Lobbyeinstellungen **(** in Kürze verfügbar ) ist eine Richtlinie pro Organisator,  die steuert, ob der [Besprechungsorganisator](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) die Lobbyeinstellungen außer Kraft setzen kann, die ein Administrator **unter** Automatisches Zulassen von Personen festgelegt hat, und Zulassen, dass Einwahlbenutzer die Lobby umgehen, wenn sie eine neue Besprechung planen.</span><span class="sxs-lookup"><span data-stu-id="7e92a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7e92a-118">**Hinweis:** Eine vollständige Übersicht über Microsoft Teams-Besprechungsrichtlinien finden Sie unter Verwalten von Besprechungsrichtlinien [in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="7e92a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
