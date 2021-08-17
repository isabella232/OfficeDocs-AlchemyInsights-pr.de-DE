---
title: So aktivieren Sie gehostete Voicemail
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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055553"
---
# <a name="how-to-enable-hosted-voicemail"></a>So aktivieren Sie gehostete Voicemail

Um Voicemail zu aktivieren, muss **HostedVoicemail** auf $true festgelegt werden.

Die **HostedVoicemail-Eigenschaft** für den Benutzer mithilfe von Remote PowerShell (RPS).

Weitere Informationen zum Herstellen einer Verbindung mit RPS finden Sie [in Microsoft Teams PowerShell-Übersicht,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) um weitere Informationen zum Herstellen einer Verbindung mit RPS zu finden.

1. Der Teams-Administrator sollte für Teams bei Remote-PowerShell angemeldet sein.
1. Über PowerShell-Aufforderung kann der Teams Administrator **set-csuser user@contoso.com -HostedVoiceMail $true** ausführen, in dem sich der SIP-URI des betreffenden Benutzers befindet.

> [!NOTE]
> Es kann bis zu 24 Stunden dauern, bis Änderungen an Richtlinien repliziert wurden.