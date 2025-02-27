---
title: Einstellungen für Besprechungsrichtlinien
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
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925164"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Verwalten von Besprechungsrichtlinien in Microsoft Teams

**Hinweis: Es kann bis zu 24 Stunden dauern, bis Richtlinienänderungen für Benutzer wirksam werden.** Möglicherweise können Sie änderungen an neu erstellten Richtlinien nicht sofort vornehmen. warten Sie 4 Stunden, und versuchen Sie erneut, eine neu erstellte Richtlinie zu ändern.

Besprechungsrichtlinien werden verwendet, um die Features zu steuern, die Besprechungsteilnehmern für Besprechungen, die von Benutzern in Ihrer Organisation geplant werden, zur Verfügung stehen. Einige Features von Besprechungsrichtlinien sind möglicherweise noch nicht im Teams Admin Center implementiert (diese werden in der Dokumentation als "bald verfügbar" bezeichnet). In diesem Fall oder wenn Sie im Microsoft Teams Admin Center einen Fehler wie "Wir können die Richtlinie derzeit nicht aktualisieren, aber später erneut versuchen" erhalten, empfehlen wir, PowerShell zum Erstellen oder Ändern Teams Besprechungsrichtlinien zu verwenden. 

Weitere Informationen zu Besprechungsrichtlinien finden Sie in den folgenden Ressourcen:

- Informationen zum Erstellen von Richtlinien, Zum Vornehmen von Änderungen und zum Zuweisen von Benutzern zur Richtlinie finden Sie unter [Verwalten von Besprechungsrichtlinien in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Informationen zum Vornehmen von Richtlinienänderungen mithilfe von PowerShell-Cmdlets finden Sie [unter Teams PowerShell-Übersicht.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Sie müssen das [Skype for Business PowerShell-Modul](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) für Teams Besprechungsrichtlinien verwenden. 
    - Weitere Informationen finden Sie in der [Dokumentation zu *-CsTeamsMeetingPolicy-Cmdlets.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

