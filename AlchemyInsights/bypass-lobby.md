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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654255"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Steuern der Lobby Einstellungen und Grad der Teilnahme

Wenn Sie möchten, dass jeder, einschließlich Einwahl, externen und anonymen Benutzern, die Lobby umgehen kann, können Sie dies mithilfe von PowerShell tun. Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Dieses Cmdlet erfordert derzeit die Verwendung Skype for Business PowerShell-Moduls. Informationen zum Einrichten der Verwendung dieses Cmdlets finden Sie unter [Managing Policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Sie können eine neue Richtlinie einrichten, die Sie dann auf Benutzer anwenden müssen. Wenn Sie die globale Richtlinie ändern, wird Sie automatisch auf Benutzer angewendet. Bei jeder Richtlinienänderung müssen Sie mindestens 4 Stunden warten, bis die Richtlinien wirksam werden.

Lesen Sie unbedingt die nachfolgende Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Grundlegendes zu Teams Besprechung Lobby Richtlinien Kontrollen

- [Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.

- [Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.

- [Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .

- [Organisatoren das außer Kraft setzen von Lobby Einstellungen erlauben](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator in **automatisch Personen** eingegeben und **Einwahl zulassen Benutzer können die Lobby umgehen,** Wenn Sie eine neue Besprechung planen.

**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen.
