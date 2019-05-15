---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057712"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="eea9a-102">Elemente können nicht gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="eea9a-102">Unable to delete items</span></span>

<span data-ttu-id="eea9a-103">Haben Sie Probleme beim Löschen von Elementen?</span><span class="sxs-lookup"><span data-stu-id="eea9a-103">Having issues deleting items?</span></span>

- <span data-ttu-id="eea9a-104">Stellen Sie immer sicher, dass Sie über die [entsprechenden Berechtigungen](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) zum Löschen des Elements verfügen, oder wenn der [Websitesammlungsadministrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) versucht, das Element zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="eea9a-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="eea9a-105">Stellen Sie sicher, dass keine [Aufbewahrungsrichtlinie](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) für das Element vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="eea9a-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="eea9a-106">Stellen Sie sicher, dass das Element nicht an einen anderen Benutzer [ausgecheckt](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.</span><span class="sxs-lookup"><span data-stu-id="eea9a-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="eea9a-107">Schließlich können Administratoren [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) verwenden, die eine Bibliothek mit PowerShell-Befehlen enthalten, mit denen Sie komplexe Verwaltungsaktionen wie das Erzwingen des Löschens von hartnäckigen Elementen ausführen.</span><span class="sxs-lookup"><span data-stu-id="eea9a-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="eea9a-108">PNP-Datei entfernen</span><span class="sxs-lookup"><span data-stu-id="eea9a-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="eea9a-109">PNP-Ordner entfernen</span><span class="sxs-lookup"><span data-stu-id="eea9a-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="eea9a-110">PNP-Listenelement entfernen</span><span class="sxs-lookup"><span data-stu-id="eea9a-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="eea9a-111">PNP-Liste entfernen</span><span class="sxs-lookup"><span data-stu-id="eea9a-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="eea9a-112">PNP-Feld entfernen (Spalte)</span><span class="sxs-lookup"><span data-stu-id="eea9a-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)