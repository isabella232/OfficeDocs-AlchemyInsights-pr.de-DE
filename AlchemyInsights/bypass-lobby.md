---
title: Umgehungs Lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684949"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Steuern von Lobby Einstellungen und Grad der Teilnahme an Teams

Wenn Sie möchten, dass jeder, einschließlich Einwahl, externen und anonymen Benutzern, **die Lobby umgehen**kann, verwenden Sie PowerShell, um diese Aufgabe auszuführen. Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Dieses Cmdlet erfordert derzeit die Verwendung Skype for Business PowerShell-Moduls. Informationen zum Einrichten für die Verwendung dieses Cmdlets finden Sie unter [Managing Policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Nachdem Sie eine Richtlinie eingerichtet haben, müssen Sie Sie auf die Benutzer anwenden. oder wenn Sie die globale Richtlinie geändert haben, wird Sie automatisch auf Benutzer angewendet. Bei jeder Richtlinienänderung müssen Sie mindestens **4 Stunden bis zu 24 Stunden** warten, bis die Richtlinien wirksam werden. 

Lesen Sie unbedingt die nachfolgende Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Grundlegendes zu Teams Besprechung Lobby Richtlinien Kontrollen

Mit diesen Einstellungen wird gesteuert, welche Besprechungsteilnehmer in der Lobby warten, bevor Sie zur Besprechung zugelassen werden, und die Teilnahmestufe, die Sie in einer Besprechung zulässig sind. Sie können PowerShell verwenden, um Besprechungsrichtlinien Einstellungen zu aktualisieren, die noch nicht implementiert wurden (mit der Bezeichnung "Coming Soon") im Teamadministrator Center. Im folgenden finden Sie ein Beispiel für ein PowerShell-Cmdlet, das es allen Benutzern ermöglicht, die Lobby zu umgehen.

- [Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.

- [Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.

- [Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .

- [Organisatoren erlauben, Lobby Einstellungen außer Kraft zu setzen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**), ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator festgelegt hat, um Benutzer **automatisch** zuzulassen und **Einwahl Benutzern die Umgehung der Lobby zu ermöglichen** , wenn Sie eine neue Besprechung planen.

**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen.
