---
title: Workflow wird nicht gestartet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403742"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="478b4-102">Workflow wird nicht gestartet</span><span class="sxs-lookup"><span data-stu-id="478b4-102">Workflow is not starting</span></span>

- <span data-ttu-id="478b4-103">SharePoint 2010- und SharePoint 2013-Workflows werden nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="478b4-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="478b4-104">Wenn Der Workflow nicht gestartet wird, kann es zu einem temporären Dienstproblem kommen, bei dem Benutzer zeitweise Verzögerungen mit dem Workflowfortschritt erleben können.</span><span class="sxs-lookup"><span data-stu-id="478b4-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="478b4-105">Überprüfen Sie [das Dienstintehashboard,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) um zu sehen, ob Ihre Organisation betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="478b4-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="478b4-106">Wenn seit dem ersten Problem mehr als 24 Stunden vergangen sind, protokollieren Sie bitte ein Supportticket.</span><span class="sxs-lookup"><span data-stu-id="478b4-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="478b4-107">In vielen Fällen arbeiten wir bereits an einer Lösung.</span><span class="sxs-lookup"><span data-stu-id="478b4-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="478b4-108">Bitte geben Sie uns mindestens 24 Stunden Zeit, um eine Lösung zu vervollständigen.</span><span class="sxs-lookup"><span data-stu-id="478b4-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="478b4-109">SharePoint 2010-Workflows verzögerten sich beim Start.</span><span class="sxs-lookup"><span data-stu-id="478b4-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="478b4-110">Dies tritt auf, wenn der Workflow in großen Batches ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="478b4-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="478b4-111">(z. B. wenn mehrere Elemente gleichzeitig hinzugefügt werden).</span><span class="sxs-lookup"><span data-stu-id="478b4-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="478b4-112">Workflows sind nicht so konzipiert, dass sie in Echtzeit ausgeführt werden, daher ist eine Verzögerung ein by-design-Verhalten.</span><span class="sxs-lookup"><span data-stu-id="478b4-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="478b4-113">Wenn der Workflow eine komplexe Extensible Object Markup Language (XMOL) ist, kann die Kompilierung langsam sein.</span><span class="sxs-lookup"><span data-stu-id="478b4-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="478b4-114">Lesen [Sie diesen](https://support.microsoft.com//kb/3043697) Artikel.</span><span class="sxs-lookup"><span data-stu-id="478b4-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="478b4-115">Sie sollten den Workflow vereinfachen oder mithilfe des Microsoft SharePoint 2013-Workflowplattformtyps neu gestalten.</span><span class="sxs-lookup"><span data-stu-id="478b4-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="478b4-116">Wenn Ihr Workflowverlauf größer geworden ist, können Sie die Elemente löschen oder eine neue Verlaufsliste erstellen.</span><span class="sxs-lookup"><span data-stu-id="478b4-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="478b4-117">Weitere Informationen : [Löschen des Workflowverlaufs](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="478b4-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="478b4-118">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="478b4-118">Related topics</span></span>
<span data-ttu-id="478b4-119">Möchten Sie Microsoft Flow in SharePoint Online testen?</span><span class="sxs-lookup"><span data-stu-id="478b4-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="478b4-120">Erstellen von Fluss</span><span class="sxs-lookup"><span data-stu-id="478b4-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="478b4-121">SharePoint und Fluss</span><span class="sxs-lookup"><span data-stu-id="478b4-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
