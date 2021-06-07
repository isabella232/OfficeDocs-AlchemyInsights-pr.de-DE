---
title: Aktivieren von Teams-Webinaren
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760837"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="fa9fe-102">Aktivieren von Teams-Webinaren</span><span class="sxs-lookup"><span data-stu-id="fa9fe-102">Enable Teams Webinars</span></span>

<span data-ttu-id="fa9fe-103">Webinare sind standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-103">Webinars are enabled by default.</span></span> <span data-ttu-id="fa9fe-104">Mithilfe der Teams PowerShell-Befehlen können Sie verwalten, wer Teams-Webinare planen und sich für diese registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="fa9fe-105">Alle Benutzer, die Besprechungen erstellen können, können auch Webinarbesprechungen erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="fa9fe-106">Um zu verwalten, wer Teams-Webinare planen kann, verwenden Sie *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="fa9fe-107">Standardmäßig ist *WhoCanRegister* aktiviert und auf **Jeder** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="fa9fe-108">Wenn Sie die Besprechungsregistrierung deaktivieren möchten, legen Sie *AllowMeetingRegistration* auf **False** fest.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="fa9fe-109">Um diese Einstellungen zu ändern, müssen Sie [Teams PowerShell](/microsoftteams/teams-powershell-install) installieren.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="fa9fe-110">Außerdem werden Besprechungsrichtlinien in Teams-Webinaren erzwungen.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="fa9fe-111">Wenn der anonyme Beitritt beispielsweise in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="fa9fe-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="fa9fe-112">Weitere Informationen dazu, wie Sie konfigurieren können, wer sich für Webinare registrieren kann, finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="fa9fe-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="fa9fe-113">Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="fa9fe-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>