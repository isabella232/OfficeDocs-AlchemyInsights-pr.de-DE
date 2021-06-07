---
title: Verwalten der Webinarregistrierung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783140"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="714b6-102">Verwalten der Webinarregistrierung</span><span class="sxs-lookup"><span data-stu-id="714b6-102">Manage webinar registration</span></span>

<span data-ttu-id="714b6-103">Sie verwalten mithilfe von Teams PowerShell-Befehlen, wer sich für Teams-Webinare registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="714b6-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="714b6-104">Informationen zum Installieren von Teams PowerShell finden Sie unter [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="714b6-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="714b6-105">Standardmäßig ist *WhoCanRegister* aktiviert und auf **EveryoneInCompany** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="714b6-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="714b6-106">Damit sich jeder, einschließlich anonymer Benutzer, registrieren kann, müssen Sie die Besprechungsrichtlinie mithilfe des PowerShell-Befehls auf **Jeder** festlegen:</span><span class="sxs-lookup"><span data-stu-id="714b6-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="714b6-107">**Hinweis**: Wenn der anonyme Beitritt in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="714b6-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="714b6-108">Weitere Informationen und die Aktivierung dieser Einstellung finden Sie unter [Verwalten von Besprechungseinstellungen in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="714b6-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="714b6-109">Wenn Sie die Besprechungsregistrierung deaktivieren möchten, legen Sie *AllowMeetingRegistration* auf **False** fest.</span><span class="sxs-lookup"><span data-stu-id="714b6-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="714b6-110">Weitere Informationen dazu, wie Sie konfigurieren können, wer sich für Webinare registrieren kann, finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="714b6-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="714b6-111">Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="714b6-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
