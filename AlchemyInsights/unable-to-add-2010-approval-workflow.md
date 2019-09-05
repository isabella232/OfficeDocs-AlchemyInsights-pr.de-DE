---
title: 2010-Genehmigungs Workflow kann nicht hinzugefügt werden
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748683"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="4a12f-102">2010-Genehmigungs Workflow kann nicht hinzugefügt werden</span><span class="sxs-lookup"><span data-stu-id="4a12f-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="4a12f-103">In einer Microsoft SharePoint-Websitesammlung können Sie einer Liste oder Bibliothek keinen Global wiederverwendbaren Workflow (beispielsweise "Genehmigungs SharePoint 2010") hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="4a12f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="4a12f-104">Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="4a12f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="4a12f-105">Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="4a12f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="4a12f-106">Wählen Sie unter **Website Objekte**die Option **Workflows**aus.</span><span class="sxs-lookup"><span data-stu-id="4a12f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="4a12f-107">Wählen Sie im **neuen** Abschnitt des Menübands **Workflows** die Option **wieder verwendbarer Workflow**aus.</span><span class="sxs-lookup"><span data-stu-id="4a12f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="4a12f-108">Geben Sie im Formular **wiederverwendbaren Workflow erstellen** den Namen \* \* *Repair2010* \* \* ein.</span><span class="sxs-lookup"><span data-stu-id="4a12f-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="4a12f-109">Klicken Sie unter **Plattformtyp**auf **SharePoint 2010 Workflow**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="4a12f-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="4a12f-110">Wählen Sie im Abschnitt **Speichern** des Menübands **Workflow** die Option **veröffentlichen**aus.</span><span class="sxs-lookup"><span data-stu-id="4a12f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="4a12f-111">Wählen Sie im Abschnitt **Manage** des Menübands **Workflow** die Option **Global veröffentlichen**aus.</span><span class="sxs-lookup"><span data-stu-id="4a12f-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="4a12f-112">Wählen Sie im daraufhin angezeigten Dialogfeld Bestätigung die Option **OK**aus.</span><span class="sxs-lookup"><span data-stu-id="4a12f-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="4a12f-113">Suchen Sie in einem Webbrowser die Stammwebsite der Websitesammlung, und greifen Sie dann auf Website **Sammlungs Features**für **Websiteeinstellungen** \> zu.</span><span class="sxs-lookup"><span data-stu-id="4a12f-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="4a12f-114">Umschalten des **Workflows** -Features:</span><span class="sxs-lookup"><span data-stu-id="4a12f-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="4a12f-115">· Wenn das Feature *aktiviert* ist, klicken Sie auf Deaktivieren **,** und klicken Sie dann auf **aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="4a12f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="4a12f-116">· Wenn das Feature *deaktiviert* ist, klicken Sie auf **aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="4a12f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="4a12f-117">Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="4a12f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

