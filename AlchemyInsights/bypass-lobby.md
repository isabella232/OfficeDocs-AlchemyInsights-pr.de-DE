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
# <a name="control-lobby-settings-and-level-of-participation"></a>Steuern der Lobby Einstellungen und Grad der Teilnahme

Mit diesen Einstellungen wird gesteuert, welche Besprechungsteilnehmer in der Lobby warten, bevor Sie zur Besprechung zugelassen werden, und die Teilnahmestufe, die Sie in einer Besprechung zulässig sind. Sie können PowerShell verwenden, um Besprechungsrichtlinien Einstellungen zu aktualisieren, die noch nicht implementiert wurden (mit der Bezeichnung "Coming Soon") im Teamadministrator Center.  Im folgenden finden Sie ein Beispiel für ein PowerShell-Cmdlet, das es allen Benutzern ermöglicht, die Lobby zu umgehen.  

- [Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis Sie von einem authentifizierten Benutzer zugelassen werden.

- [Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine Richtlinie auf Organisatoren, die steuert, ob anonyme Personen, einschließlich B2B-und Verbundbenutzern, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer von der Organisation angehört.

- [Zulassen, dass Einwahlbenutzer die Lobby umgehen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organisator, die steuert, ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung **Personen automatisch zulassen** .

- [Organisatoren das außer Kraft setzen von Lobby Einstellungen erlauben](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (in**Kürze**verfügbar) ist eine Richtlinie pro Organizer, die steuert, ob der Besprechungsorganisator die Lobby Einstellungen außer Kraft setzen kann, die ein Administrator in **automatisch Personen** eingegeben und **Einwahl zulassen Benutzer können die Lobby umgehen,** Wenn Sie eine neue Besprechung planen.

**Hinweis:** Lesen Sie [Manage Meeting Policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , um eine vollständige Übersicht über die Microsoft Teams-Besprechungsrichtlinien zu bekommen. 


**PowerShell-Beispiel**

Wenn Sie allen, einschließlich externen oder anonymen Benutzern, erlauben möchten, die Lobby zu umgehen, können Sie diese Aufgabe auch mithilfe von PowerShell ausführen.  Hier sehen Sie ein Beispiel für die Änderung der globalen Besprechungsrichtlinie für Ihre Organisation.   

(Lesen Sie unbedingt die obige Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.)

Festlegen-CsTeamsMeetingPolicy-Identity Global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $true

Weitere Informationen finden Sie unter [Sets-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
