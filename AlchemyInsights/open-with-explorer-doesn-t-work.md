---
title: Mit Explorer öffnen funktioniert nicht
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469511"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c799a-102">Mit Explorer öffnen ist nicht funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="c799a-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c799a-p101">Falls **mit Explorer öffnen** oder **im Datei-Explorer-Ansicht** nicht funktioniert stellen Sie sicher, dass der WebClient-Dienst **ausgeführt** wird durch die folgenden Schritte. Beispielsweise könnte dauert lange, bis eine Bibliothek für SharePoint oder OneDrive geöffnet wird, wenn der Dienst nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c799a-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c799a-105">Klicken Sie im Suchfeld Windows Typ ausführen, wählen Sie ausführen-desktop-app, geben Sie Services.msc ein, und wählen Sie dann **EINGABETASTE**.</span><span class="sxs-lookup"><span data-stu-id="c799a-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c799a-p102">Führen Sie einen Bildlauf nach unten zu den WebClient-Dienst, und überprüfen Sie die Spalte **Status** . Ist der Status der WebClient-Dienst nicht **ausgeführt wird**, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. Aktivieren Sie den Dienst bei Bedarf, indem Sie in **der Liste Starttyp** **manuell** oder **automatisch** auswählen.</span><span class="sxs-lookup"><span data-stu-id="c799a-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c799a-p103">Zum Beheben von Startproblemen im Datei-Explorer öffnen finden Sie unter [im Explorer öffnen](https://go.microsoft.com/fwlink/?linkid=871665). Erkunden Sie die Synchronisierung als bessere Alternative: [Synchronisierung SharePoint-Dateien mit der neuen OneDrive Sync-Client](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c799a-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

