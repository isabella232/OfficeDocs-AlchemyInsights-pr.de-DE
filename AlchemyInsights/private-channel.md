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
# <a name="private-channels-in-microsoft-teams"></a>Private Kanäle in Microsoft Teams

Private Kanäle ist ein neues Feature in Microsoft Teams. Beachten Sie, dass private Kanäle nicht von Standardkanälen konvertiert werden können oder umgekehrt.

Ausführliche Informationen zu privaten Kanälen wie Informationen zur [privaten Kanalerstellung und Mitgliedschaft](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) sowie zu [privaten Kanal-SharePoint-Websites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)finden Sie unter private Channels [in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Hinweis:** Da die Konfiguration für die Aufbewahrung privater Kanal Nachrichten noch nicht unterstützt wird, sind für Mandanten mit aktivierten Aufbewahrungsrichtlinien keine privaten Kanäle standardmäßig aktiviert. Private Kanäle können im Teamadministrator Center aktiviert werden. Beachten Sie außerdem, dass die Aufbewahrung von in privaten Kanälen freigegebenen Dateien unterstützt wird, während die Aufbewahrung privater Kanal Nachrichten nicht unterstützt wird.

**Benötigen Sie einen neuen Teambesitzer?**

Wenn Ihr privater Kanalbesitzer verlässt, können Sie einen neuen Teambesitzer über Teams PowerShell hinzufügen.


- Klicken Sie [hier](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , um Microsoft Teams PowerShell zu installieren.

Das folgende Cmdlet wird benötigt:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Weitere Informationen zu Teams PowerShell finden Sie unter [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
