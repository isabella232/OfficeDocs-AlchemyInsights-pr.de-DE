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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376645"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="70ffe-102">Steuern der Lobby Einstellungen und Grad der Teilnahme</span><span class="sxs-lookup"><span data-stu-id="70ffe-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="70ffe-103">Mit diesen Einstellungen wird gesteuert, welche Besprechungsteilnehmer in der Lobby warten, bevor Sie zur Besprechung zugelassen werden, und die Teilnahmestufe, die Sie in einer Besprechung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="70ffe-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="70ffe-104">Sie können PowerShell verwenden, um Besprechungsrichtlinien Einstellungen zu aktualisieren, die noch nicht implementiert wurden (mit der Bezeichnung "Coming Soon") im Teamadministrator Center.</span><span class="sxs-lookup"><span data-stu-id="70ffe-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="70ffe-105">Im folgenden finden Sie ein Beispiel für ein PowerShell-Cmdlet, das es allen Benutzern ermöglicht, die Lobby zu umgehen.</span><span class="sxs-lookup"><span data-stu-id="70ffe-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="70ffe-106">[Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.</span><span class="sxs-lookup"><span data-stu-id="70ffe-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="70ffe-107">[Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.</span><span class="sxs-lookup"><span data-stu-id="70ffe-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="70ffe-108">[Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .</span><span class="sxs-lookup"><span data-stu-id="70ffe-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="70ffe-109">[Organisatoren das außer Kraft setzen von Lobby Einstellungen erlauben](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator in **automatisch Personen** eingegeben und **Einwahl zulassen Benutzer können die Lobby umgehen,** Wenn Sie eine neue Besprechung planen.</span><span class="sxs-lookup"><span data-stu-id="70ffe-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="70ffe-110">**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen.</span><span class="sxs-lookup"><span data-stu-id="70ffe-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="70ffe-111">**PowerShell-Beispiel**</span><span class="sxs-lookup"><span data-stu-id="70ffe-111">**PowerShell example**</span></span>

<span data-ttu-id="70ffe-112">Wenn Sie allen, einschließlich externen oder anonymen Benutzern, erlauben möchten, die Lobby zu umgehen, können Sie diese Aufgabe auch mithilfe von PowerShell ausführen.</span><span class="sxs-lookup"><span data-stu-id="70ffe-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="70ffe-113">Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="70ffe-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="70ffe-114">(Lesen Sie unbedingt die obige Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.)</span><span class="sxs-lookup"><span data-stu-id="70ffe-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="70ffe-115">Festlegen-CsTeamsMeetingPolicy-Identity Global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $true</span><span class="sxs-lookup"><span data-stu-id="70ffe-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="70ffe-116">Weitere Informationen finden Sie unter [Sets-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="70ffe-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
