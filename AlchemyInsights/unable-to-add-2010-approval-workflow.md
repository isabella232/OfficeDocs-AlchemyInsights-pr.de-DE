---
title: Kann nicht für einen Genehmigungsworkflow 2010 hinzugefügt werden
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470435"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="b1c18-102">Kann nicht für einen Genehmigungsworkflow 2010 hinzugefügt werden</span><span class="sxs-lookup"><span data-stu-id="b1c18-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="b1c18-103">Sie können nicht in einer Microsoft SharePoint-Websitesammlung ein Global wieder verwendbaren Workflows (beispielsweise "Genehmigung - SharePoint 2010") zu einer Liste oder Bibliothek hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b1c18-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b1c18-104">Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="b1c18-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b1c18-105">Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b1c18-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b1c18-106">Wählen Sie unter **Standortobjekten** **Workflows**aus.</span><span class="sxs-lookup"><span data-stu-id="b1c18-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b1c18-107">Wählen Sie im Abschnitt **neu** des Menübands **Workflows** **Wieder Verwendbarer Workflow**aus.</span><span class="sxs-lookup"><span data-stu-id="b1c18-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b1c18-p101">Klicken Sie auf das Formular **Wieder verwendbaren Workflow erstellen** , geben Sie den Namen \*\* *Repair2010* \*\*. Klicken Sie auf **SharePoint 2010-Workflows**für **Plattformtyp**und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="b1c18-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="b1c18-110">Aktivieren Sie im Abschnitt **Speichern** des Menübands **Workflow** **Veröffentlichen**.</span><span class="sxs-lookup"><span data-stu-id="b1c18-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="b1c18-p102">Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** **Global veröffentlichen**. Klicken Sie im Dialogfeld Bestätigung wählen Sie **OK**aus.</span><span class="sxs-lookup"><span data-stu-id="b1c18-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="b1c18-p103">In einem Webbrowser die Stammwebsite der Websitesammlung zu suchen, und klicken Sie dann auf zugreifen **Site Settings** \> **Websitesammlungs-Features**. Schalten Sie das Feature **Workflows** :</span><span class="sxs-lookup"><span data-stu-id="b1c18-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b1c18-115">· Wenn das Feature *aktiviert* ist, klicken Sie auf **deaktivieren,** und klicken Sie dann auf **Aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="b1c18-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b1c18-116">· Wenn das Feature *deaktiviert* ist, klicken Sie auf **Aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="b1c18-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b1c18-117">Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b1c18-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

