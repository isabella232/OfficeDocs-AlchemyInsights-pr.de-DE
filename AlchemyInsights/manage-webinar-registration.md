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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798643"
---
# <a name="manage-webinar-registration"></a>Verwalten der Webinarregistrierung

Sie verwalten mithilfe von Teams PowerShell-Befehlen, wer sich für Teams-Webinare registrieren kann. Informationen zum Installieren von Teams PowerShell finden Sie unter [Teams PowerShell](/microsoftteams/teams-powershell-install). 

Standardmäßig ist *WhoCanRegister* aktiviert und auf **Jeder** festgelegt. 

Wenn in der Besprechungseinladung die Option, die Registrierung für jeden zuzulassen, nicht angezeigt wird, legen Sie *WhoCanRegister* erneut auf „Jeder“ fest, und warten Sie 24 Stunden. Zum erneuten Ausführen von *WhoCanRegister* verwenden Sie den PowerShell-Befehl:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Hinweis**: Wenn der anonyme Beitritt in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen. Weitere Informationen und die Aktivierung dieser Einstellung finden Sie unter [Verwalten von Besprechungseinstellungen in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Wenn Sie die Besprechungsregistrierung deaktivieren möchten, legen Sie *AllowMeetingRegistration* auf **False** fest.

Weitere Informationen dazu, wie Sie konfigurieren können, wer sich für Webinare registrieren kann, finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](/sharepoint/control-lists).
