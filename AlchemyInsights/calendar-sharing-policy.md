---
title: 618 Kalenderfreigabe Richtlinie
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684229"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="6c478-102">Richtlinienfehler beim Freigeben eines Kalenders</span><span class="sxs-lookup"><span data-stu-id="6c478-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="6c478-103">Führen Sie entsprechend ihrer Situation eine der folgenden Aktionen aus:</span><span class="sxs-lookup"><span data-stu-id="6c478-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="6c478-104">Stellen Sie mithilfe von Remote-PowerShell eine Verbindung zu Exchange Online her.</span><span class="sxs-lookup"><span data-stu-id="6c478-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="6c478-105">Weitere Informationen finden Sie unter [Herstellen einer Verbindung mit Exchange Online mithilfe von Remote-PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6c478-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="6c478-106">Öffnen Sie auf dem lokalen Server das Exchange-Verwaltungsshell.</span><span class="sxs-lookup"><span data-stu-id="6c478-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="6c478-107">Bestimmen Sie die Freigaberichtlinie, die dem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="6c478-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="6c478-108">Führen Sie dazu den folgenden Befehl aus, und beachten Sie die zurückgegebene Richtlinie:</span><span class="sxs-lookup"><span data-stu-id="6c478-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="6c478-109">Aktualisieren Sie die Freigaberichtlinie für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="6c478-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="6c478-110">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="6c478-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="6c478-111">Öffnen Sie das Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="6c478-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="6c478-112">Klicken Sie auf **Organisation**, und doppelklicken Sie dann auf die Richtlinie, die dem Benutzer unter **individuelle Freigabe**zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="6c478-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="6c478-113">Dies ist die Richtlinie, die in Schritt 2 zurückgegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="6c478-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="6c478-114">Wählen Sie auf der Seite Freigabe Regel die Kalenderfreigabe Ebene aus, die Sie zulassen möchten unter Geben Sie an, **welche Informationen Sie freigeben**möchten. Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="6c478-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="6c478-115">Weitere Informationen finden Sie unter: ["die Richtlinie erlaubt nicht das Erteilen von Berechtigungen auf dieser Ebene für einen oder mehrere Empfänger Fehler, wenn der Benutzer versucht, Kalender freizugeben](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="6c478-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
