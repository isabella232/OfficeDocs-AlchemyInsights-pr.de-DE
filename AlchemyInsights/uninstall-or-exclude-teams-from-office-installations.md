---
title: Deinstallieren oder Ausschließen von Teams aus Office-Installationen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010298"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Deinstallieren oder Ausschließen von Teams aus neuen oder vorhandenen Office-Installationen

Microsoft Teams ist im Rahmen von Microsoft 365 apps for Enterprise, Microsoft 365 apps for Business und Office für Mac enthalten.

- Verwenden Sie das [Office-Bereitstellungs Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , um Teams von neuen Office-Installationen auszuschließen.
- Informationen zum *deinstallieren* von Teams von einem Gerät mit Windows finden Sie unter [Deinstallieren von Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Informationen zum Bereinigen von Microsoft Teams von mehreren Zielcomputern oder Benutzern finden Sie unter [Bereinigung der Microsoft Teams-Bereitstellung](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Verwenden Sie die [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -Option, um zu verhindern, dass Microsoft Teams automatisch mit Office installiert wird.
- Verwenden Sie *vor dem Installieren*von Microsoft Teams die Option [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , um zu verhindern, dass Microsoft Teams nach der Installation automatisch gestartet wird.

Wenn Sie Office für Mac verwenden, finden Sie weitere Informationen unter [Microsoft Teams-Installationen auf einem Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).