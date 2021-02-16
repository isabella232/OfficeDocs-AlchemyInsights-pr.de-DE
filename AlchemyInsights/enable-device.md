---
title: Gerät aktivieren
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255161"
---
# <a name="enable-device"></a>Gerät aktivieren

**So aktivieren Sie das Gerät mithilfe des Befehls "Powershell"**

Führen Sie die folgenden Befehle aus:

- So erhalten Sie das Geräteobjekt: `Get-MsolDevice -Name <Name>`
- So aktivieren Sie das Gerät: `Enable-MsolDevice -DeviceId <DeviceId>`

Weitere Informationen zum Konfigurieren des Hybrid join für verwaltete Domänen finden Sie unter [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
