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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768439"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Steuern der Lobby Einstellungen und Grad der Teilnahme

Wenn Sie möchten, dass jeder, einschließlich Einwahl, externen und anonymen Benutzern, die Lobby in Microsoft Teams umgehen kann, können Sie dies mithilfe von PowerShell tun. Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Dieses Cmdlet erfordert derzeit die Verwendung Skype for Business PowerShell-Moduls. Informationen zum Einrichten der Verwendung dieses Cmdlets finden Sie unter [Managing Policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Sie können eine neue Richtlinie einrichten, die Sie dann auf Benutzer anwenden müssen. Wenn Sie die globale Richtlinie ändern, wird Sie automatisch auf Benutzer angewendet. Bei jeder Richtlinienänderung müssen Sie mindestens 4 Stunden warten, bis die Richtlinien wirksam werden.

Lesen Sie unbedingt die nachfolgende Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Grundlegendes zu Teams Besprechung Lobby Richtlinien Kontrollen

- [Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.

- [Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.

- [Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .

- [Organisatoren erlauben, Lobby Einstellungen außer Kraft zu setzen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**), ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator festgelegt hat, um Benutzer **automatisch** zuzulassen und **Einwahl Benutzern die Umgehung der Lobby zu ermöglichen** , wenn Sie eine neue Besprechung planen.

**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen.
