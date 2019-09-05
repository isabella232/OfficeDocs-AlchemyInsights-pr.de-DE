---
title: Behandeln von Problemen bei "Mit Explorer öffnen" in SharePoint Online
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 73583b3b27143c708a4cc993cdff94a33131ab52
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36743092"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="c3271-102">Behandeln von Problemen bei "Mit Explorer öffnen" in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c3271-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="c3271-103">Mit dem Befehl „Mit Explorer öffnen“ wird eine lokale Instanz von Windows Explorer geöffnet, die die Ordnerstruktur auf dem Server anzeigt, auf dem sich die SharePoint-Website befindet.</span><span class="sxs-lookup"><span data-stu-id="c3271-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="c3271-104">In diesem Fall empfiehlt es sich, die [Synchronisierung von SharePoint-Dateien mit dem neuen OneDrive-Synchronisierungsclient](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> durchzuführen, der [Dateien bei Bedarf](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) bereitstellt, da er lokalen Zugriff auf Ihre Dateien und die optimale Leistung bietet.</span><span class="sxs-lookup"><span data-stu-id="c3271-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="c3271-105">Wenn Sie die Explorer-Ansicht dem neuen OneDrive-Synchronisierungsclient vorziehen, stellen Sie sicher, dass Sie die in den folgenden Artikeln aufgeführten Schritte und bewährten Methoden befolgen:</span><span class="sxs-lookup"><span data-stu-id="c3271-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="c3271-106">Verwenden des Befehls „Mit Explorer öffnen“ zum Beheben von Problemen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c3271-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- <span data-ttu-id="c3271-107">[Kopieren oder Verschieben von Bibliotheksdateien mit dem Befehl „Mit Explorer öffnen“](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="c3271-107">See [Video: Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2).</span></span>

> [!Note]  
> <span data-ttu-id="c3271-108">Die Schaltfläche **Mit Explorer öffnen** wird in der neuen Bibliotheksoberfläche nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c3271-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="c3271-109">Klicken Sie auf das Dropdownmenü **Ansicht** in der oberen rechten Ecke (der Name der Dropdownliste ist abhängig von der aktuellen Ansicht) und klicken Sie dann auf **Im Datei-Explorer anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="c3271-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="c3271-110">Der Befehl „Mit Explorer öffnen“ in SharePoint verwendet ActiveX-Steuerelemente und wird deshalb nur in Internet Explorer 10 oder 11 unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3271-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="c3271-111">„Mit Explorer öffnen“ kann unter Windows nicht mit Microsoft Edge, Google Chrome oder Mozilla Firefox und auch nicht auf der Mac-Plattform verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c3271-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="c3271-112">Aus diesem Grund ist die Option „Im Explorer anzeigen“ möglicherweise ausgegraut.</span><span class="sxs-lookup"><span data-stu-id="c3271-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="c3271-113">[Warum SharePoint-Menübandschaltflächen nicht verfügbar oder ausgegraut sind.](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="c3271-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

