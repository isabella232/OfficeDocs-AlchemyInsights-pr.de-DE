---
title: Grenzwert für tägliche e-Mail überschritten. Workflow ist angehalten.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514450"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="924b3-103">Grenzwert für tägliche e-Mail überschritten.</span><span class="sxs-lookup"><span data-stu-id="924b3-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="924b3-104">Workflow ist angehalten.</span><span class="sxs-lookup"><span data-stu-id="924b3-104">Workflow is suspended.</span></span>

<span data-ttu-id="924b3-105">Dieser Fehler kann in den folgenden Szenarien eingegangen sein:</span><span class="sxs-lookup"><span data-stu-id="924b3-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="924b3-106">Sie verfügen über einen Workflow in SharePoint Online, der den SharePoint 2010 oder SharePoint 2013 Workflow-Plattformtyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="924b3-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="924b3-107">Der Workflow ist so konfiguriert, dass eine benutzerdefinierte e-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig gesendet wird, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute.</span><span class="sxs-lookup"><span data-stu-id="924b3-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="924b3-108">Wenn Sie den Workflow ausführen, wird die e-Mail-Nachricht nicht gesendet, und Sie sehen das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="924b3-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="924b3-109">Für einen Workflow mithilfe des SharePoint 2013 Plattformtyps navigieren Sie zur Seite **Workflow Status** .</span><span class="sxs-lookup"><span data-stu-id="924b3-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="924b3-110">Auf der Seite Workflow Status ist der **interne Status** auf **gestartet**festgelegt, und die Informations Sprechblase zeigt an, dass **keine Empfänger gesendet**werden können.</span><span class="sxs-lookup"><span data-stu-id="924b3-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="924b3-111">Um dieses Problem zu umgehen, konfigurieren Sie Ihren Workflow zum Senden von e-Mail-Nachrichten, ohne die [Exchange Online Absender Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)zu überschreiten.</span><span class="sxs-lookup"><span data-stu-id="924b3-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="924b3-112">Verwenden Sie beispielsweise eine Pause im Workflow, senden Sie die e-Mail an eine Office 365 Gruppe, eine Verteilergruppe oder eine e-Mail-aktivierte Sicherheitsgruppe, oder senden Sie die Nachricht an weniger als 200 Empfänger gleichzeitig.</span><span class="sxs-lookup"><span data-stu-id="924b3-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="924b3-113">Weitere Informationen finden Sie im folgenden [Artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="924b3-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="924b3-114">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="924b3-114">Related topics</span></span>
- [<span data-ttu-id="924b3-115">Fluss erstellen</span><span class="sxs-lookup"><span data-stu-id="924b3-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="924b3-116">SharePoint und Flow</span><span class="sxs-lookup"><span data-stu-id="924b3-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 