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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Steuern der Lobbyeinstellungen und des Grads der Teilnahme an Teams

Wenn Sie allen Benutzern, einschließlich Einwahlbenutzern, externen und anonymen Benutzern, erlauben möchten, die Lobby zu **umgehen,** verwenden Sie PowerShell, um diese Aufgabe zu erledigen. Hier sehen Sie ein Beispiel für das Ändern der globalen Besprechungsrichtlinie für Ihre Organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Dieses Cmdlet erfordert derzeit die Verwendung des Skype for Business PowerShell-Moduls. Informationen zur Einrichtung für die Verwendung dieses Cmdlets erhalten Sie unter [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Nachdem Sie eine Richtlinie eingerichtet haben, müssen Sie sie auf Benutzer anwenden. oder, wenn Sie die globale Richtlinie geändert haben, gilt sie automatisch für Benutzer. Für jede Richtlinienänderung müssen Sie mindestens 4 Stunden bis **zu 24** Stunden warten, bis die Richtlinien wirksam werden. 

Lesen Sie unbedingt die unten aufgeführte Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Grundlegendes zu Richtliniensteuerelementen für Besprechungslobbys in Teams

Diese Einstellungen steuern, welche Besprechungsteilnehmer in der Lobby warten, bevor sie zur Besprechung zugelassen werden, und welche Teilnehmer an einer Besprechung teilnehmen dürfen. Sie können PowerShell verwenden, um Besprechungsrichtlinieneinstellungen zu aktualisieren, die noch nicht implementiert wurden (mit der Bezeichnung "bald verfügbar") im Teams Admin Center. Ein Beispiel für ein PowerShell-Cmdlet, mit dem alle Benutzer die Lobby umgehen können, finden Sie unten.

- [Die automatische Zulassung](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) von Personen ist eine Richtlinie pro Organisator, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder in der Lobby warten, bis sie von einem authentifizierten Benutzer zugelassen werden.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Das Starten einer Besprechung durch anonyme Personen ist eine Richtlinie pro Organisator, die steuert, ob anonyme Personen, einschließlich B2B- und Verbundbenutzer, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer aus der Organisation anwesend ist.

- Zulassen, dass Einwahlbenutzer die Lobby [(](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) in Kürze **)** umgehen, ist eine Richtlinie pro Organisator, die steuert,  ob Personen, die sich per Telefon einwählen, direkt an der Besprechung teilnehmen oder in der Lobby warten, unabhängig von der Einstellung Personen automatisch zulassen.

- Organisatoren das Außerkraft setzen von Lobbyeinstellungen **(** in Kürze verfügbar ) ist eine Richtlinie pro Organisator,  die steuert, ob der [Besprechungsorganisator](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) die Lobbyeinstellungen außer Kraft setzen kann, die ein Administrator **unter** Automatisches Zulassen von Personen festgelegt hat, und Zulassen, dass Einwahlbenutzer die Lobby umgehen, wenn sie eine neue Besprechung planen.

**Hinweis:** Eine vollständige Übersicht über Microsoft Teams-Besprechungsrichtlinien finden Sie unter Verwalten von Besprechungsrichtlinien [in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)
