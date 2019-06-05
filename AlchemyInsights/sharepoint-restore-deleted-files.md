---
title: Wiederherstellen einer gelöschten Datei oder eines gelöschten Ordners
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: d5250d75a982c0afc9d3e1b2a43be2ba9c3e8f59
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716506"
---
## <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="53d86-102">Wiederherstellen einer gelöschten Datei oder eines gelöschten Ordners</span><span class="sxs-lookup"><span data-stu-id="53d86-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="53d86-103">SharePoint Online behält Sicherungen aller Inhalte für 14 zusätzliche Tage außerhalb des tatsächlichen Löschvorgangs bei.</span><span class="sxs-lookup"><span data-stu-id="53d86-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="53d86-104">Wenn Inhalte nicht über den Papierkorb oder die Wiederherstellung von Dateien wiederhergestellt werden können, kann ein Administrator sich an den Microsoft-Support wenden, um eine Wiederherstellung innerhalb des 14-tägigen Fensters anzufordern.</span><span class="sxs-lookup"><span data-stu-id="53d86-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="53d86-105">Wiederherstellungen von Sicherungen können nur für Websitesammlungen oder Unterwebsites ausgeführt werden, nicht für bestimmte Dateien, Listen oder Bibliotheken.</span><span class="sxs-lookup"><span data-stu-id="53d86-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="53d86-106">Wenn Sie ein Element oder eine Website aus SharePoint löschen, wird es nicht sofort entfernt.</span><span class="sxs-lookup"><span data-stu-id="53d86-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="53d86-107">Gelöschte Elemente wechseln für einen bestimmten Zeitraum in den Papierkorb.</span><span class="sxs-lookup"><span data-stu-id="53d86-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="53d86-108">Während dieser Zeit können Sie die gelöschten Elemente an Ihrem ursprünglichen Speicherort wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="53d86-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="53d86-109">Weitere Informationen finden Sie unter den Links unten.</span><span class="sxs-lookup"><span data-stu-id="53d86-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="53d86-110">[Wiederherstellen von Elementen im Papierkorb einer SharePoint-Website](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="53d86-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="53d86-111">Wiederherstellen gelöschter Dateien oder Ordner in OneDrive</span><span class="sxs-lookup"><span data-stu-id="53d86-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/en-us/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="53d86-112">Wiederherstellen einer gelöschten Websitesammlung (einschließlich Gruppen-, Kommunikations-und anderen Websites)</span><span class="sxs-lookup"><span data-stu-id="53d86-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="53d86-113">Wiederherstellen einer gelöschten OneDrive-Website</span><span class="sxs-lookup"><span data-stu-id="53d86-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/en-us/onedrive/restore-deleted-onedrive)

<span data-ttu-id="53d86-114">Für Massen Papierkorb Aktionen können Administratoren die Verwendung von [SharePoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)in Frage stellen.</span><span class="sxs-lookup"><span data-stu-id="53d86-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

## <a name="files-restore-feature"></a><span data-ttu-id="53d86-115">Datei Wiederherstellung (Feature)</span><span class="sxs-lookup"><span data-stu-id="53d86-115">Files Restore feature</span></span>

<span data-ttu-id="53d86-116">Wenn viele ihrer OneDrive-oder SharePoint-Dateien gelöscht, überschrieben, beschädigt oder durch Schadsoftware infiziert werden, können Sie die gesamte OneDrive-oder SharePoint-Bibliothek mit dem Feature zum Wiederherstellen der Dateien in einem früheren Zeitpunkt wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="53d86-116">If lots of your OneDrive or Sharepoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="53d86-117">Wiederherstellen einer OneDrive-Bibliothek</span><span class="sxs-lookup"><span data-stu-id="53d86-117">Restore a OneDrive library</span></span>](https://support.office.com/en-us/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="53d86-118">Wiederherstellen einer Dokumentbibliothek</span><span class="sxs-lookup"><span data-stu-id="53d86-118">Restore a Document library</span></span>](https://support.office.com/en-us/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

