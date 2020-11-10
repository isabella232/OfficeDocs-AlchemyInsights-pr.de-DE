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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="deed3-102">Verwenden von Giphys in Microsoft Teams-Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="deed3-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="deed3-103">Giphys-Zugriff in Microsoft Teams Chat ist standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="deed3-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="deed3-104">Als Administrator können Sie steuern, ob Giphys für Benutzer verfügbar sind, indem Sie [eine Messagingrichtlinie festlegen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) und sicherstellen, dass die **Verwendung von Giphys in Unterhaltungen** **eingeschaltet** ist.</span><span class="sxs-lookup"><span data-stu-id="deed3-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="deed3-105">Wenn GIFs in Microsoft Teams-Unterhaltungen nicht erwartungsgemäß funktionieren, überprüfen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="deed3-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="deed3-106">Die [Messagingrichtlinie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muss Giphys zulassen.</span><span class="sxs-lookup"><span data-stu-id="deed3-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="deed3-107">So überprüfen Sie mithilfe von PowerShell-Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="deed3-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="deed3-108">Stellen Sie sicher, dass Sie [Teams mit PowerShell verwalten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)können.</span><span class="sxs-lookup"><span data-stu-id="deed3-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="deed3-109">Führen Sie den PowerShell-Befehl [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) aus, und stellen Sie sicher, dass **AllowGiphy** auf **true** festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="deed3-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="deed3-110">Wenn **AllowGiphy** auf **false** festgelegt ist, führen Sie den folgenden PowerShell-Befehlssatz aus [– CsTeamsMessagingPolicy-Identity Global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="deed3-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="deed3-111">[Optionale verbundene Benutzeroberflächen](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) müssen aktiviert sein, um den Zugriff auf die Giphy-URL zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="deed3-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="deed3-112">Wenn Sie mehrere Teams-Messaging Richtlinien für Ihren Mandanten konfiguriert haben, können Sie die Identität der Richtlinie ermitteln, die dem betroffenen Benutzer mit dem PowerShell-Befehl [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | zugewiesen ist. <user@domain.com> Wählen Sie TeamsMessagingPolicy aus.</span><span class="sxs-lookup"><span data-stu-id="deed3-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
