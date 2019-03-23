---
title: Mit Explorer öffnen funktioniert nicht
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764907"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="90060-102">Mit Explorer öffnen funktioniert nicht</span><span class="sxs-lookup"><span data-stu-id="90060-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="90060-103">Wenn **mit Explorer** oder **Ansicht im Datei-Explorer** öffnen nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst **ausgeführt** wird, indem Sie die folgenden Schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="90060-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="90060-104">Beispielsweise kann es sehr viel Zeit in Anspruch nehmen, eine SharePoint-oder OneDrive-Bibliothek zu öffnen, wenn der Dienst nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="90060-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="90060-105">Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Option Desktop ausführen aus, geben Sie Services. msc ein, und drücken Sie die **EINGABETASTE**.</span><span class="sxs-lookup"><span data-stu-id="90060-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="90060-106">Scrollen Sie nach unten zum webClient-Dienst, und überprüfen Sie die Spalte **Status** .</span><span class="sxs-lookup"><span data-stu-id="90060-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="90060-107">Wenn der webClient-Dienststatus nicht **aktiv**ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="90060-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="90060-108">Aktivieren Sie den Dienst, falls erforderlich, indem Sie im Feld Starttyp entweder \*\*\*\* **manuell** oder **automatisch** auswählen.</span><span class="sxs-lookup"><span data-stu-id="90060-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="90060-109">Informationen zur Problembehandlung beim Öffnen im Datei-Explorer finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="90060-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="90060-110">UnterSuchen Sie die Synchronisierung als bessere Alternative: [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="90060-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

