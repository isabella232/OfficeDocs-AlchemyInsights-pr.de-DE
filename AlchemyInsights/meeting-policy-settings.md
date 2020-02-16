---
title: Besprechungsrichtlinien Einstellungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042843"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="7b76f-102">Verwalten von Besprechungsrichtlinien in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7b76f-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="7b76f-103">**Hinweis: Es kann bis zu 24 Stunden dauern, bis Richtlinienänderungen für Benutzer wirksam werden.**</span><span class="sxs-lookup"><span data-stu-id="7b76f-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="7b76f-104">Möglicherweise können Sie nicht sofort Änderungen an neu erstellten Richtlinien vornehmen. warten Sie 4 Stunden, und versuchen Sie erneut, eine neu erstellte Richtlinie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="7b76f-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="7b76f-105">Besprechungsrichtlinien werden verwendet, um die Features zu steuern, die Besprechungsteilnehmern für Besprechungen zur Verfügung stehen, die von Benutzern in Ihrer Organisation geplant werden.</span><span class="sxs-lookup"><span data-stu-id="7b76f-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="7b76f-106">Einige Features von Besprechungsrichtlinien werden möglicherweise noch nicht in der Microsoft Teams-Verwaltungskonsole implementiert (diese werden in der Dokumentation mit "Coming Soon" bezeichnet).</span><span class="sxs-lookup"><span data-stu-id="7b76f-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="7b76f-107">In diesem Fall oder wenn Sie eine Fehlermeldung wie "Wir können die Richtlinie jetzt nicht aktualisieren, aber später wiederholen" im Microsoft Teams Admin Center erhalten, empfehlen wir die Verwendung von PowerShell zum Erstellen oder Ändern von Besprechungsrichtlinien für Teams.</span><span class="sxs-lookup"><span data-stu-id="7b76f-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="7b76f-108">Weitere Informationen zu Besprechungsrichtlinien finden Sie in den folgenden Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="7b76f-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="7b76f-109">Informationen zum Erstellen von Richtlinien, zum vornehmen von Änderungen und zum Zuweisen von Benutzern zur Richtlinie finden Sie unter [Manage Meeting Policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="7b76f-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="7b76f-110">Informationen zum vornehmen von Richtlinienänderungen mithilfe von PowerShell-Cmdlets finden Sie unter [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="7b76f-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="7b76f-111">Sie müssen das [Skype for Business PowerShell-Modul](https://www.microsoft.com/download/details.aspx?id=39366) für Teams-Besprechungsrichtlinien verwenden.</span><span class="sxs-lookup"><span data-stu-id="7b76f-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="7b76f-112">Weitere Informationen finden Sie in der [Dokumentation zur \*-CsTeamsMeetingPolicy-Cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="7b76f-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

