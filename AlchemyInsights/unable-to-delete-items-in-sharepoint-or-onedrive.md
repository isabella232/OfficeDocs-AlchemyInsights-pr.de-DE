---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049516"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="8525f-102">Elemente können nicht gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="8525f-102">Unable to delete items</span></span>

<span data-ttu-id="8525f-103">Probleme beim Löschen von SharePoint-Elementen?</span><span class="sxs-lookup"><span data-stu-id="8525f-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="8525f-104">Stellen Sie immer sicher, dass Sie über die [entsprechenden Berechtigungen](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) zum Löschen des Elements verfügen oder wenn ein [Websitesammlungsadministrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) versucht, das Element zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="8525f-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="8525f-105">Stellen Sie sicher, dass kein [Aufbewahrungsrichtlinien](https://docs.microsoft.com/office365/securitycompliance/retention-policies) Setup für das Element vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="8525f-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="8525f-106">Stellen Sie sicher, dass das Element nicht für einen anderen Benutzer [ausgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.</span><span class="sxs-lookup"><span data-stu-id="8525f-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="8525f-107">Schließlich können Administratoren [SharePoint-Muster und-Methoden](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) verwenden, das eine Bibliothek mit PowerShell-Befehlen enthält, mit denen Sie komplexe Verwaltungsaktionen wie das Löschen hartnäckiger Elemente erzwingen können.</span><span class="sxs-lookup"><span data-stu-id="8525f-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="8525f-108">PNP-Datei entfernen</span><span class="sxs-lookup"><span data-stu-id="8525f-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="8525f-109">PNP-Ordner entfernen</span><span class="sxs-lookup"><span data-stu-id="8525f-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="8525f-110">PNP-Listenelement entfernen</span><span class="sxs-lookup"><span data-stu-id="8525f-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="8525f-111">PNP-Liste entfernen</span><span class="sxs-lookup"><span data-stu-id="8525f-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="8525f-112">PNP-Feld entfernen (Spalte)</span><span class="sxs-lookup"><span data-stu-id="8525f-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)