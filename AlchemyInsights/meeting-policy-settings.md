---
title: Einstellungen für Besprechungsrichtlinien
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704605"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="1ea38-102">Verwalten von Besprechungsrichtlinien in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1ea38-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="1ea38-103">**Hinweis: Es kann bis zu 24 Stunden dauern, bis Richtlinienänderungen für Benutzer wirksam werden.**</span><span class="sxs-lookup"><span data-stu-id="1ea38-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="1ea38-104">Möglicherweise können Sie änderungen an neu erstellten Richtlinien nicht sofort vornehmen. warten Sie 4 Stunden, und versuchen Sie erneut, eine neu erstellte Richtlinie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="1ea38-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="1ea38-105">Besprechungsrichtlinien werden verwendet, um die Features zu steuern, die Besprechungsteilnehmern für Besprechungen zur Verfügung stehen, die von Benutzern in Ihrer Organisation geplant werden.</span><span class="sxs-lookup"><span data-stu-id="1ea38-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="1ea38-106">Einige Features von Besprechungsrichtlinien sind möglicherweise noch nicht im Teams Admin Center implementiert (diese werden in der Dokumentation als "in Kürze" bezeichnet).</span><span class="sxs-lookup"><span data-stu-id="1ea38-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="1ea38-107">In diesem Fall oder wenn Sie im Microsoft Teams Admin Center einen Fehler wie "Wir können die Richtlinie derzeit nicht aktualisieren, aber später erneut testen" erhalten, wird empfohlen, PowerShell zum Erstellen oder Ändern von Teams-Besprechungsrichtlinien zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="1ea38-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="1ea38-108">Weitere Informationen zu Besprechungsrichtlinien finden Sie in den folgenden Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="1ea38-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="1ea38-109">Weitere Informationen zum Erstellen von Richtlinien, zum Vornehmen von Änderungen und zum Zuweisen von Benutzern zur Richtlinie finden Sie unter [Verwalten von Besprechungsrichtlinien in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="1ea38-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="1ea38-110">Informationen zum Vornehmen von Richtlinienänderungen mithilfe von PowerShell-Cmdlets finden Sie unter [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="1ea38-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="1ea38-111">Sie müssen das [Skype for Business PowerShell-Modul für](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams-Besprechungsrichtlinien verwenden.</span><span class="sxs-lookup"><span data-stu-id="1ea38-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="1ea38-112">Weitere Informationen finden Sie in der Dokumentation zu [\*-CsTeamsMeetingPolicy-Cmdlets.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="1ea38-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

