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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798643"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="21a29-102">Verwalten der Webinarregistrierung</span><span class="sxs-lookup"><span data-stu-id="21a29-102">Manage webinar registration</span></span>

<span data-ttu-id="21a29-103">Sie verwalten mithilfe von Teams PowerShell-Befehlen, wer sich für Teams-Webinare registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="21a29-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="21a29-104">Informationen zum Installieren von Teams PowerShell finden Sie unter [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="21a29-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="21a29-105">Standardmäßig ist *WhoCanRegister* aktiviert und auf **Jeder** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21a29-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="21a29-106">Wenn in der Besprechungseinladung die Option, die Registrierung für jeden zuzulassen, nicht angezeigt wird, legen Sie *WhoCanRegister* erneut auf „Jeder“ fest, und warten Sie 24 Stunden.</span><span class="sxs-lookup"><span data-stu-id="21a29-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="21a29-107">Zum erneuten Ausführen von *WhoCanRegister* verwenden Sie den PowerShell-Befehl:</span><span class="sxs-lookup"><span data-stu-id="21a29-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="21a29-108">**Hinweis**: Wenn der anonyme Beitritt in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="21a29-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="21a29-109">Weitere Informationen und die Aktivierung dieser Einstellung finden Sie unter [Verwalten von Besprechungseinstellungen in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="21a29-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="21a29-110">Wenn Sie die Besprechungsregistrierung deaktivieren möchten, legen Sie *AllowMeetingRegistration* auf **False** fest.</span><span class="sxs-lookup"><span data-stu-id="21a29-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="21a29-111">Weitere Informationen dazu, wie Sie konfigurieren können, wer sich für Webinare registrieren kann, finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="21a29-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="21a29-112">Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="21a29-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
