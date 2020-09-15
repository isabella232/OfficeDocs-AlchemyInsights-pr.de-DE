---
title: Deinstallieren oder Ausschließen von Teams aus Office-Installationen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658220"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="9ad33-102">Deinstallieren oder Ausschließen von Teams aus neuen oder vorhandenen Office-Installationen</span><span class="sxs-lookup"><span data-stu-id="9ad33-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="9ad33-103">Microsoft Teams ist im Rahmen von Microsoft 365 apps for Enterprise, Microsoft 365 apps for Business und Office für Mac enthalten.</span><span class="sxs-lookup"><span data-stu-id="9ad33-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="9ad33-104">Verwenden Sie das [Office-Bereitstellungs Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , um Teams von neuen Office-Installationen auszuschließen.</span><span class="sxs-lookup"><span data-stu-id="9ad33-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="9ad33-105">Informationen zum *deinstallieren* von Teams von einem Gerät mit Windows finden Sie unter [Deinstallieren von Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="9ad33-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="9ad33-106">Informationen zum Bereinigen von Microsoft Teams von mehreren Zielcomputern oder Benutzern finden Sie unter [Bereinigung der Microsoft Teams-Bereitstellung](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="9ad33-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="9ad33-107">Verwenden Sie die [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -Option, um zu verhindern, dass Microsoft Teams automatisch mit Office installiert wird.</span><span class="sxs-lookup"><span data-stu-id="9ad33-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="9ad33-108">Verwenden Sie *vor dem Installieren*von Microsoft Teams die Option [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , um zu verhindern, dass Microsoft Teams nach der Installation automatisch gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="9ad33-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="9ad33-109">Wenn Sie Office für Mac verwenden, finden Sie weitere Informationen unter [Microsoft Teams-Installationen auf einem Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="9ad33-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>