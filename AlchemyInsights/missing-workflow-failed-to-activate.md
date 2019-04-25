---
title: FehlEnder Workflow konnte nicht aktiviert werden
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418432"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="97088-102">FehlEnder Workflow konnte nicht aktiviert werden</span><span class="sxs-lookup"><span data-stu-id="97088-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="97088-103">In einer Microsoft SharePoint-Websitesammlung können Sie einer Liste oder Bibliothek keinen Global wiederverwendbaren Workflow (wie "Genehmigungs-SharePoint 2010") hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="97088-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="97088-104">Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="97088-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="97088-105">Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="97088-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="97088-106">Wählen Sie unter **Website Objekte**die Option **Workflows**aus.</span><span class="sxs-lookup"><span data-stu-id="97088-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="97088-107">Wählen Sie im Abschnitt **neu** des Menübands **Workflows** **wieder verwendbarer Workflow**aus.</span><span class="sxs-lookup"><span data-stu-id="97088-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="97088-108">Geben Sie im Formular **wieder verwendbare Workflows erstellen** den Namen \* \* *Repair2010* \* \* ein.</span><span class="sxs-lookup"><span data-stu-id="97088-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="97088-109">Klicken Sie unter **Plattformtyp**auf **sharePoint 2010-Workflow**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="97088-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="97088-110">Wählen Sie im **Workflow** -Menüband im Abschnitt **Speichern** die Option **veröffentlichen**aus.</span><span class="sxs-lookup"><span data-stu-id="97088-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="97088-111">Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** die Option **Global veröffentlichen**aus.</span><span class="sxs-lookup"><span data-stu-id="97088-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="97088-112">Klicken Sie im daraufhin angezeigten Bestätigungsdialogfeld auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="97088-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="97088-113">Navigieren Sie in einem Webbrowser zu der Stammwebsite der Websitesammlung, und greifen Sie dann auf Website **Sammlungs Features**für **Websiteeinstellungen** \> zu.</span><span class="sxs-lookup"><span data-stu-id="97088-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="97088-114">Aktivieren Sie dann das Feature **Workflows** :</span><span class="sxs-lookup"><span data-stu-id="97088-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="97088-115">· Wenn das Feature *aktiviert* ist, klicken Sie auf Deaktivieren **,** und klicken Sie dann auf **aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="97088-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="97088-116">· Wenn das Feature *deaktiviert* ist, klicken Sie auf **aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="97088-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="97088-117">Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="97088-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

