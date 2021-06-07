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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760832"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="dee44-102">Verwalten der Webinarregistrierung</span><span class="sxs-lookup"><span data-stu-id="dee44-102">Manage webinar registration</span></span>

<span data-ttu-id="dee44-103">Mithilfe der Teams PowerShell-Befehlen können Sie verwalten, wer sich für Teams-Webinare registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="dee44-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="dee44-104">Standardmäßig ist *WhoCanRegister* aktiviert und auf **Jeder** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="dee44-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="dee44-105">Wenn Sie die Besprechungsregistrierung deaktivieren möchten, legen Sie *AllowMeetingRegistration* auf **False** fest.</span><span class="sxs-lookup"><span data-stu-id="dee44-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="dee44-106">Um diese Einstellungen zu ändern, müssen Sie [Teams PowerShell](/microsoftteams/teams-powershell-install) installieren.</span><span class="sxs-lookup"><span data-stu-id="dee44-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="dee44-107">Außerdem werden Besprechungsrichtlinien in Teams-Webinaren erzwungen.</span><span class="sxs-lookup"><span data-stu-id="dee44-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="dee44-108">Wenn der anonyme Beitritt beispielsweise in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="dee44-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="dee44-109">Weitere Informationen dazu, wie Sie konfigurieren können, wer sich für Webinare registrieren kann, finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="dee44-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="dee44-110">Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="dee44-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>