---
title: Behandeln von Problemen bei "Mit Explorer öffnen" in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086047"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="fca85-102">Behandeln von Problemen bei „Mit Explorer öffnen“ in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fca85-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="fca85-103">Folgen Sie den Schritten und bewährten Methoden in den unten stehenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="fca85-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="fca85-104">Verwenden des Befehls „Mit Explorer öffnen“ zum Beheben von Problemen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fca85-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="fca85-105">Kopieren oder Verschieben von Bibliotheksdateien mit dem Befehl „Mit Explorer öffnen“</span><span class="sxs-lookup"><span data-stu-id="fca85-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="fca85-106">Es empfiehlt sich, die [Synchronisierung von Microsoft Office SharePoint Online-Dateien mit dem neuen OneDrive-Synchronisierungsclient](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) durchzuführen, der [Dateien bei Bedarf](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) bereitstellt, da er lokalen Zugriff auf Ihre Dateien und eine optimale Leistung bietet.</span><span class="sxs-lookup"><span data-stu-id="fca85-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="fca85-107">**Mit Explorer öffnen** wird nur in Internet Explorer 11 unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fca85-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="fca85-108">Weitere Informationen finden Sie unter [Ende des Supports von IE11 für Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy).</span><span class="sxs-lookup"><span data-stu-id="fca85-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="fca85-109">**Mit Explorer öffnen** kann unter Windows nicht mit Microsoft Edge, Google Chrome oder Mozilla Firefox und auch nicht auf der Mac-Plattform verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="fca85-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="fca85-110">Aus diesem Grund ist die Option **Im Explorer anzeigen** möglicherweise ausgegraut.</span><span class="sxs-lookup"><span data-stu-id="fca85-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="fca85-111">Die Schaltfläche **Mit Explorer öffnen** wird in der neuen Bibliotheksoberfläche nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fca85-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="fca85-112">Klicken Sie auf das Dropdownmenü **Ansicht** in der oberen rechten Ecke (der Name der Dropdownliste ist abhängig von der aktuellen Ansicht), und klicken Sie dann auf **Im Datei-Explorer anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="fca85-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

