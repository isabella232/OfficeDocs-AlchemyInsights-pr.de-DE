---
title: Verwenden von Giphys in Microsoft Teams-Unterhaltungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947516"
---
# <a name="using-giphys-in-teams-conversations"></a>Verwenden von Giphys in Microsoft Teams-Unterhaltungen

Giphys-Zugriff in Microsoft Teams Chat ist standardmäßig aktiviert. Als Administrator können Sie steuern, ob Giphys für Benutzer verfügbar sind, indem Sie [eine Messagingrichtlinie festlegen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) und sicherstellen, dass die **Verwendung von Giphys in Unterhaltungen** **eingeschaltet** ist.

Wenn GIFs in Microsoft Teams-Unterhaltungen nicht erwartungsgemäß funktionieren, überprüfen Sie Folgendes:

Die [Messagingrichtlinie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muss Giphys zulassen. So überprüfen Sie mithilfe von PowerShell-Cmdlets:

- Stellen Sie sicher, dass Sie [Teams mit PowerShell verwalten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)können.
- Führen Sie den PowerShell-Befehl [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) aus, und stellen Sie sicher, dass **AllowGiphy** auf **true** festgelegt ist.
- Wenn **AllowGiphy** auf **false** festgelegt ist, führen Sie den folgenden PowerShell-Befehlssatz aus [– CsTeamsMessagingPolicy-Identity Global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Optionale verbundene Benutzeroberflächen](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) müssen aktiviert sein, um den Zugriff auf die Giphy-URL zu ermöglichen.

> [!NOTE]
> Wenn Sie mehrere Teams-Messaging Richtlinien für Ihren Mandanten konfiguriert haben, können Sie die Identität der Richtlinie ermitteln, die dem betroffenen Benutzer mit dem PowerShell-Befehl [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | zugewiesen ist. <user@domain.com> Wählen Sie TeamsMessagingPolicy aus.
