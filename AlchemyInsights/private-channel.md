---
title: Privater Kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005437"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="1ff46-102">Private Kanäle in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1ff46-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="1ff46-103">Private Kanäle ist ein neues Feature in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1ff46-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="1ff46-104">Beachten Sie, dass private Kanäle nicht von Standardkanälen konvertiert werden können oder umgekehrt.</span><span class="sxs-lookup"><span data-stu-id="1ff46-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="1ff46-105">Ausführliche Informationen zu privaten Kanälen wie Informationen zur [privaten Kanalerstellung und Mitgliedschaft](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) sowie zu [privaten Kanal-SharePoint-Websites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)finden Sie unter private Channels [in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="1ff46-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="1ff46-106">**Hinweis:** Da die Konfiguration für die Aufbewahrung privater Kanal Nachrichten noch nicht unterstützt wird, sind für Mandanten mit aktivierten Aufbewahrungsrichtlinien keine privaten Kanäle standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1ff46-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="1ff46-107">Private Kanäle können im Teamadministrator Center aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="1ff46-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="1ff46-108">Beachten Sie außerdem, dass die Aufbewahrung von in privaten Kanälen freigegebenen Dateien unterstützt wird, während die Aufbewahrung privater Kanal Nachrichten nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="1ff46-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="1ff46-109">**Benötigen Sie einen neuen Teambesitzer?**</span><span class="sxs-lookup"><span data-stu-id="1ff46-109">**Need a new team owner?**</span></span>

<span data-ttu-id="1ff46-110">Wenn Ihr privater Kanalbesitzer verlässt, können Sie einen neuen Teambesitzer über Teams PowerShell hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1ff46-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="1ff46-111">Klicken Sie [hier](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , um Microsoft Teams PowerShell zu installieren.</span><span class="sxs-lookup"><span data-stu-id="1ff46-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="1ff46-112">Das folgende Cmdlet wird benötigt:</span><span class="sxs-lookup"><span data-stu-id="1ff46-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="1ff46-113">Weitere Informationen zu Teams PowerShell finden Sie unter [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="1ff46-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
