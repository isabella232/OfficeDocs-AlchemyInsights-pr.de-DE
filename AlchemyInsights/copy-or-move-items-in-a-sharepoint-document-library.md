---
title: Kopieren oder verlagern von Elementen in einer SharePoint-Dokumentbibliothek
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 5/24/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: 6e14260d3670eb15f73e92dc5b0c86e0e842974a
ms.sourcegitcommit: efdde3c24a0c1adfb8b6f5f59dcae435fb5c53a8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/19/2019
ms.locfileid: "38711755"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="9422e-102">Kopieren oder verlagern von Elementen in einer SharePoint-Dokumentbibliothek</span><span class="sxs-lookup"><span data-stu-id="9422e-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="9422e-103">Sie können Dateien, Ordner und Links an unterschiedliche Speicherorte in einer Dokumentbibliothek kopieren und dort verlagern.</span><span class="sxs-lookup"><span data-stu-id="9422e-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="9422e-104">Sie können auch Elemente über Websites hinweg kopieren.</span><span class="sxs-lookup"><span data-stu-id="9422e-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="9422e-105">Navigieren Sie in einem Browser zu den Dateien, Ordnern oder Links, die Sie wechseln möchten, und klicken Sie dann auf **Kopieren in** oder **wechseln Sie zu**.</span><span class="sxs-lookup"><span data-stu-id="9422e-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9422e-106">" **Kopieren in** " und " **in" umsteigen** "sind nicht verfügbar, wenn Sie die klassische Erfahrung von SharePoint Online verwenden.</span><span class="sxs-lookup"><span data-stu-id="9422e-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="9422e-107">Wählen Sie unter **Ziel auswählen**den Speicherort aus, an den Sie die Elemente kopieren oder verlagern möchten, oder klicken Sie auf **Websites Durchsuchen** , um die vollständige Liste der Websites anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9422e-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9422e-108">Wenn beim Kopieren von Elementen keine anderen Websites aufgeführt werden, wurde das Kopieren zwischen Websites nicht konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="9422e-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="9422e-109">Navigieren Sie zur Seite Einstellungen im SharePoint Admin Center, und klicken Sie auf **OK**, um es zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="9422e-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="9422e-110">Um einen neuen Ordner zu erstellen, wählen Sie einen Speicherort in der Ordnerhierarchie aus, klicken Sie auf **neuer Ordner**, geben Sie einen Namen für den Ordner ein, und klicken Sie auf das Häkchen, um den Namen zu speichern.</span><span class="sxs-lookup"><span data-stu-id="9422e-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="9422e-111">Klicken Sie auf **hier kopieren** oder hierhin zu **Navigieren**.</span><span class="sxs-lookup"><span data-stu-id="9422e-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9422e-112">Sie können Dateien und Ordner gleichzeitig auf bis zu 500 MB kopieren.</span><span class="sxs-lookup"><span data-stu-id="9422e-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="9422e-113">> Wenn Sie Dokumente mit Versionsverlauf kopieren, wird nur die neueste Version kopiert.</span><span class="sxs-lookup"><span data-stu-id="9422e-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="9422e-114">Wenn Sie Dokumente verschieben, wird auch deren Verlauf verschoben.</span><span class="sxs-lookup"><span data-stu-id="9422e-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="9422e-115">Wenn eine Datei verschoben wird, wird Sie weiterhin im Quellverzeichnis angezeigt, bis Sie vollständig in das Ziel verschoben wurde, und dann wird Sie gelöscht.</span><span class="sxs-lookup"><span data-stu-id="9422e-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="9422e-116">Die Datei verbleiben nach Abschluss des Vorgangs im Papierkorb der Quell Websites und unterliegen dem normalen Wiederverwendungs Zeitplan, es sei denn, ein Benutzer stellt ihn aus dem Papierkorb wieder her.</span><span class="sxs-lookup"><span data-stu-id="9422e-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="9422e-117">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="9422e-117">For more information, see:</span></span>

 - <span data-ttu-id="9422e-118">[Migrieren oder Kopieren von Dateien in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Artikel zur Office-Unterstützung)</span><span class="sxs-lookup"><span data-stu-id="9422e-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="9422e-119">[Migrieren von Dateien aus einem beliebigen Ordner in Office 365](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community Blog-Artikel)</span><span class="sxs-lookup"><span data-stu-id="9422e-119">[Move files from any folder in Office 365](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  