---
title: Aktivieren von gehosteter Voicemail
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608849"
---
# <a name="how-to-enable-hosted-voicemail"></a>Aktivieren von gehosteter Voicemail

Um Voicemail zu aktivieren, muss **HostedVoicemail** auf $true festgelegt sein.

Die **HostedVoicemail** -Eigenschaft des Benutzers, der Remote-PowerShell (RPS) verwendet.

Weitere Informationen zum Herstellen einer Verbindung mit RPS finden Sie unter [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) für weitere Informationen zum Herstellen einer Verbindung mit RPS.

1. Der Microsoft Teams-Administrator sollte bei Remote-PowerShell für Teams angemeldet sein.
1. Von der PowerShell-Eingabeaufforderung aus kann der Microsoft Teams-Administrator die **Csuser-user@contoso.com-HostedVoiceMail-$true** ausführen, in der der SIP-URI des betreffenden Benutzers vorliegt.

> [!NOTE]
> Änderungen an Richtlinien können bis zu 24 Stunden dauern, bis Sie repliziert werden.