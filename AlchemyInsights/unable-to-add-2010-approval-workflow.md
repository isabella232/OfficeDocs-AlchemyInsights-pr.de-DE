---
title: 2010-Genehmigungs Workflow kann nicht hinzugefügt werden
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699734"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="f1cce-102">2010-Genehmigungs Workflow kann nicht hinzugefügt werden</span><span class="sxs-lookup"><span data-stu-id="f1cce-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="f1cce-103">In einer Microsoft SharePoint-Websitesammlung können Sie einer Liste oder Bibliothek keinen Global wiederverwendbaren Workflow (beispielsweise "Genehmigungs SharePoint 2010") hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f1cce-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f1cce-104">Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="f1cce-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f1cce-105">Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f1cce-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f1cce-106">Wählen Sie unter **Website Objekte**die Option **Workflows**aus.</span><span class="sxs-lookup"><span data-stu-id="f1cce-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f1cce-107">Wählen Sie im **neuen** Abschnitt des Menübands **Workflows** die Option **wieder verwendbarer Workflow**aus.</span><span class="sxs-lookup"><span data-stu-id="f1cce-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f1cce-108">Geben Sie im Formular **wiederverwendbaren Workflow erstellen** den Namen \* \* *Repair2010* \* \* ein.</span><span class="sxs-lookup"><span data-stu-id="f1cce-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="f1cce-109">Klicken Sie unter **Plattformtyp**auf **SharePoint 2010 Workflow**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="f1cce-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f1cce-110">Wählen Sie im Abschnitt **Speichern** des Menübands **Workflow** die Option **veröffentlichen**aus.</span><span class="sxs-lookup"><span data-stu-id="f1cce-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f1cce-111">Wählen Sie im Abschnitt **Manage** des Menübands **Workflow** die Option **Global veröffentlichen**aus.</span><span class="sxs-lookup"><span data-stu-id="f1cce-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="f1cce-112">Wählen Sie im daraufhin angezeigten Dialogfeld Bestätigung die Option **OK**aus.</span><span class="sxs-lookup"><span data-stu-id="f1cce-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f1cce-113">Suchen Sie in einem Webbrowser die Stammwebsite der Websitesammlung, und greifen Sie dann auf **Site Settings** Website \> **Sammlungs Features**für Websiteeinstellungen zu.</span><span class="sxs-lookup"><span data-stu-id="f1cce-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="f1cce-114">Umschalten des **Workflows** -Features:</span><span class="sxs-lookup"><span data-stu-id="f1cce-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f1cce-115">· Wenn das Feature  *aktiviert*  ist, klicken Sie auf Deaktivieren **,** und klicken Sie dann auf **aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="f1cce-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f1cce-116">· Wenn das Feature  *deaktiviert*  ist, klicken Sie auf **aktivieren**.</span><span class="sxs-lookup"><span data-stu-id="f1cce-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f1cce-117">Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f1cce-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

