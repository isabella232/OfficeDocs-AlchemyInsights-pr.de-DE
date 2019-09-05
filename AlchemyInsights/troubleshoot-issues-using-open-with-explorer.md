---
title: Behandeln von Problemen mit "Öffnen mit Explorer"
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742732"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="c51ba-102">Beheben von Problemen mit dem Öffnen mit dem Explorer</span><span class="sxs-lookup"><span data-stu-id="c51ba-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="c51ba-103">Beheben Sie häufige Probleme beim Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mit dem Befehl **Öffnen mit Explorer** :</span><span class="sxs-lookup"><span data-stu-id="c51ba-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="c51ba-104">Verwenden Sie Internet Explorer 10 oder Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="c51ba-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="c51ba-105">**Open with Explorer** ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel.</span><span class="sxs-lookup"><span data-stu-id="c51ba-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c51ba-106">**Mit Explorer öffnen** ist in allen Browsern außer Internet Explorer deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="c51ba-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="c51ba-107">**Open with Explorer** steht in der modernen Benutzeroberfläche für SharePoint-Bibliotheken nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="c51ba-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="c51ba-108">Verwenden Sie stattdessen die **Ansicht im Datei-Explorer** .</span><span class="sxs-lookup"><span data-stu-id="c51ba-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="c51ba-109">Wählen Sie Ansichts **Optionen** \> **anzeigen im Datei-Explorer**aus.</span><span class="sxs-lookup"><span data-stu-id="c51ba-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="c51ba-110">Die Ansicht im Datei-Explorer ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel.</span><span class="sxs-lookup"><span data-stu-id="c51ba-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c51ba-111">Im **Datei-Explorer anzeigen** nur in Internet Explorer verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c51ba-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="c51ba-112">Stellen Sie sicher, dass der WebClient-Dienst aktiv ist.</span><span class="sxs-lookup"><span data-stu-id="c51ba-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="c51ba-113">Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Option Desktop-App ausführen aus, geben Sie Services. msc ein, und drücken Sie dann die EINGABETASTE.</span><span class="sxs-lookup"><span data-stu-id="c51ba-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="c51ba-114">Scrollen Sie nach unten zum WebClient Dienst, und stellen Sie sicher, dass in der Spalte **Status** die Meldung "Running" angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c51ba-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="c51ba-115">Wenn dies nicht der Fall ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="c51ba-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c51ba-116">(Möglicherweise müssen Sie den Dienst zunächst aktivieren, indem Sie im Feld **Starttyp** entweder **manuell** oder **automatisch** auswählen.)</span><span class="sxs-lookup"><span data-stu-id="c51ba-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c51ba-117">Das Öffnen einer Bibliothek im Datei-Explorer ist praktisch, wenn Sie mehrere Dateien und Ordner einmal kopieren oder umlegen müssen, aber wenn Sie regelmäßig in der Bibliothek arbeiten möchten, empfehlen wir die Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="c51ba-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="c51ba-118">Informationen zum Behandeln von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="c51ba-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c51ba-119">Informationen zum Einrichten der Synchronisierung finden Sie unter [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c51ba-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="c51ba-120">Weitere Informationen finden Sie im Artikel [Verwenden des Befehls "Open with Explorer" zur Behandlung von Problemen in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="c51ba-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

