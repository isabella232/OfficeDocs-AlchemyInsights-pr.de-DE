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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="a4c80-102">Aktivieren von gehosteter Voicemail</span><span class="sxs-lookup"><span data-stu-id="a4c80-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="a4c80-103">Um Voicemail zu aktivieren, muss **HostedVoicemail** auf $true festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="a4c80-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="a4c80-104">Die **HostedVoicemail** -Eigenschaft des Benutzers, der Remote-PowerShell (RPS) verwendet.</span><span class="sxs-lookup"><span data-stu-id="a4c80-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="a4c80-105">Weitere Informationen zum Herstellen einer Verbindung mit RPS finden Sie unter [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) für weitere Informationen zum Herstellen einer Verbindung mit RPS.</span><span class="sxs-lookup"><span data-stu-id="a4c80-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="a4c80-106">Der Microsoft Teams-Administrator sollte bei Remote-PowerShell für Teams angemeldet sein.</span><span class="sxs-lookup"><span data-stu-id="a4c80-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="a4c80-107">Von der PowerShell-Eingabeaufforderung aus kann der Microsoft Teams-Administrator die **Csuser-user@contoso.com-HostedVoiceMail-$true** ausführen, in der der SIP-URI des betreffenden Benutzers vorliegt.</span><span class="sxs-lookup"><span data-stu-id="a4c80-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="a4c80-108">Änderungen an Richtlinien können bis zu 24 Stunden dauern, bis Sie repliziert werden.</span><span class="sxs-lookup"><span data-stu-id="a4c80-108">Changes to policies can take up to 24 hours to replicate.</span></span>