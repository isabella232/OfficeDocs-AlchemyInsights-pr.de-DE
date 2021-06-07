---
title: Verwalten der Webinarregistrierung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783140"
---
# <a name="manage-webinar-registration"></a>Verwalten der Webinarregistrierung

Sie verwalten mithilfe von Teams PowerShell-Befehlen, wer sich für Teams-Webinare registrieren kann. Informationen zum Installieren von Teams PowerShell finden Sie unter [Teams PowerShell](/microsoftteams/teams-powershell-install). 

Standardmäßig ist *WhoCanRegister* aktiviert und auf **EveryoneInCompany** festgelegt. Damit sich jeder, einschließlich anonymer Benutzer, registrieren kann, müssen Sie die Besprechungsrichtlinie mithilfe des PowerShell-Befehls auf **Jeder** festlegen:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Hinweis**: Wenn der anonyme Beitritt in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen. Weitere Informationen und die Aktivierung dieser Einstellung finden Sie unter [Verwalten von Besprechungseinstellungen in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Wenn Sie die Besprechungsregistrierung deaktivieren möchten, legen Sie *AllowMeetingRegistration* auf **False** fest.

Weitere Informationen dazu, wie Sie konfigurieren können, wer sich für Webinare registrieren kann, finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](/sharepoint/control-lists).
