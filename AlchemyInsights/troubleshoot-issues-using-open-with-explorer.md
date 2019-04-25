---
title: Behandeln von Problemen beim Öffnen mit Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390606"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="512f5-102">Beheben von Problemen mit Open mit Explorer</span><span class="sxs-lookup"><span data-stu-id="512f5-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="512f5-103">Beheben häufig auftretender Probleme beim Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mit dem Befehl **Open with Explorer** :</span><span class="sxs-lookup"><span data-stu-id="512f5-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="512f5-104">Verwenden Sie Internet Explorer 10 oder Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="512f5-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="512f5-105">**Open with Explorer** ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel.</span><span class="sxs-lookup"><span data-stu-id="512f5-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="512f5-106">**Open with Explorer** ist in allen Browsern außer Internet Explorer deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="512f5-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="512f5-107">**Open with Explorer** ist in der modernen Umgebung für SharePoint-Bibliotheken nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="512f5-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="512f5-108">Verwenden Sie stattdessen die **Ansicht im Datei-Explorer** .</span><span class="sxs-lookup"><span data-stu-id="512f5-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="512f5-109">Wählen Sie **Ansichts Options** \> **Ansicht im Datei-Explorer**aus.</span><span class="sxs-lookup"><span data-stu-id="512f5-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="512f5-110">Die Ansicht im Datei-Explorer ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel.</span><span class="sxs-lookup"><span data-stu-id="512f5-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="512f5-111">**Ansicht im Datei-Explorer** in nur in Internet Explorer verfügbar.</span><span class="sxs-lookup"><span data-stu-id="512f5-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="512f5-112">Stellen Sie sicher, dass der webClient-Dienst gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="512f5-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="512f5-113">Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Option Desktop ausführen, geben Sie Services. msc ein, und drücken Sie dann die EINGABETASTE.</span><span class="sxs-lookup"><span data-stu-id="512f5-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="512f5-114">Scrollen Sie nach unten zum webClient-Dienst, und stellen Sie sicher, dass in der Spalte **Status** die Option Running angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="512f5-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="512f5-115">Wenn dies nicht der Fall ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="512f5-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="512f5-116">(Möglicherweise müssen Sie den Dienst zuerst aktivieren, indem Sie im Feld Starttyp \*\*\*\* entweder **manuell** oder **automatisch** auswählen.)</span><span class="sxs-lookup"><span data-stu-id="512f5-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="512f5-117">Das Öffnen einer Bibliothek im Datei-Explorer ist praktisch, wenn Sie mehrere Dateien und Ordner einmal kopieren oder verschieben müssen, aber wenn Sie regelmäßig in der Bibliothek arbeiten möchten, wird die Synchronisierung empfohlen.</span><span class="sxs-lookup"><span data-stu-id="512f5-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="512f5-118">Informationen zur Problembehandlung beim Öffnen im Datei-Explorer finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="512f5-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="512f5-119">Weitere Informationen zum Einrichten der Synchronisierung finden Sie unter [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="512f5-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="512f5-120">Weitere Informationen finden Sie im Artikel [Verwenden des Befehls "Öffnen mit Explorer" zur Behandlung von Problemen in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) .</span><span class="sxs-lookup"><span data-stu-id="512f5-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

