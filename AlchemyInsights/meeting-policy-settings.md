---
title: Besprechungsrichtlinien Einstellungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627573"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Verwalten von Besprechungsrichtlinien in Microsoft Teams

Besprechungsrichtlinien werden verwendet, um die Features zu steuern, die Besprechungsteilnehmern für Besprechungen zur Verfügung stehen, die von Benutzern in Ihrer Organisation geplant werden. Einige Features von Besprechungsrichtlinien werden möglicherweise noch nicht in der Microsoft Teams-Verwaltungskonsole implementiert (diese werden in der Dokumentation mit "Coming Soon" bezeichnet). In diesem Fall oder wenn Sie eine Fehlermeldung wie "Wir können die Richtlinie jetzt nicht aktualisieren, aber später wiederholen" im Microsoft Teams Admin Center erhalten, empfehlen wir die Verwendung von PowerShell zum Erstellen oder Ändern von Besprechungsrichtlinien für Teams. 

Weitere Informationen zu Besprechungsrichtlinien finden Sie in den folgenden Ressourcen:

- Informationen zum Erstellen von Richtlinien, zum vornehmen von Änderungen und zum Zuweisen von Benutzern zur Richtlinie finden Sie unter [Manage Meeting Policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Informationen zum vornehmen von Richtlinienänderungen mithilfe von PowerShell-Cmdlets finden Sie unter [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Sie müssen das [Skype for Business PowerShell-Modul](https://www.microsoft.com/download/details.aspx?id=39366) für Teams-Besprechungsrichtlinien verwenden. 
    - Weitere Informationen finden Sie in der [Dokumentation zur *-CsTeamsMeetingPolicy-Cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

**Hinweis:** Es kann bis zu 24 Stunden dauern, bis Richtlinienänderungen für Benutzer wirksam werden. Möglicherweise können Sie nicht sofort Änderungen an neu erstellten Richtlinien vornehmen. warten Sie 4 Stunden, und versuchen Sie erneut, eine neu erstellte Richtlinie zu ändern. Wenn weiterhin Probleme auftreten, versuchen Sie es mit PowerShell.  