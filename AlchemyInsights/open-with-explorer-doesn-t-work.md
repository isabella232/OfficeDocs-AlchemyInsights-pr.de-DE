---
title: "\"Mit Explorer öffnen\" funktioniert nicht"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713033"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="3afa7-102">Öffnen mit Explorer ist nicht funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="3afa7-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="3afa7-103">Wenn **Open with Explorer** oder **View im Datei-Explorer** nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst auf " **Running** " festgelegt ist, indem Sie die folgenden Schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="3afa7-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="3afa7-104">Es kann beispielsweise eine lange Zeit dauern, eine SharePoint-oder OneDrive-Bibliothek zu öffnen, wenn der Dienst nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="3afa7-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="3afa7-105">Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Desktop-App ausführen aus, geben Sie Services. msc ein, und drücken Sie die **EINGABETASTE**.</span><span class="sxs-lookup"><span data-stu-id="3afa7-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="3afa7-106">Scrollen Sie nach unten zum WebClient Dienst, und überprüfen Sie die Spalte **Status** .</span><span class="sxs-lookup"><span data-stu-id="3afa7-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="3afa7-107">Wenn der WebClient-Dienststatus nicht **aktiv**ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="3afa7-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="3afa7-108">Aktivieren Sie den Dienst, falls erforderlich, indem Sie im Feld **Starttyp** entweder **manuell** oder **automatisch** auswählen.</span><span class="sxs-lookup"><span data-stu-id="3afa7-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="3afa7-109">Informationen zum Behandeln von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="3afa7-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="3afa7-110">Durchsuchen Sie die Synchronisierung als bessere Alternative: [Synchronisieren Sie SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="3afa7-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

