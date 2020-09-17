---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806110"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="1ec18-102">Elemente können nicht gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="1ec18-102">Unable to delete items</span></span>

<span data-ttu-id="1ec18-103">Aufbewahrungsrichtlinien können dazu führen, dass Sie die entsprechenden Haltestatus, die dieses Problem verursachen, entweder deaktivieren oder ausschließen müssen.</span><span class="sxs-lookup"><span data-stu-id="1ec18-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="1ec18-104">Nach dem Entfernen einer Aufbewahrungsrichtlinie oder eines Haltestatus kann es bis zu 24 Stunden dauern, bis die Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="1ec18-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="1ec18-105">Stellen Sie sicher, dass kein [Aufbewahrungsrichtlinien](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) Setup für das Element vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="1ec18-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="1ec18-106">Die Website hat möglicherweise die Speichergrenzwerte überschritten, das [Websitekontingent](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) erhöht und das Element gelöscht.</span><span class="sxs-lookup"><span data-stu-id="1ec18-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="1ec18-107">Stellen Sie sicher, dass das Element nicht für einen anderen Benutzer [ausgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.</span><span class="sxs-lookup"><span data-stu-id="1ec18-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="1ec18-108">Schließlich können Administratoren [SharePoint-Muster und-Methoden](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) verwenden, das eine Bibliothek mit PowerShell-Befehlen enthält, mit denen Sie komplexe Verwaltungsaktionen wie das Löschen hartnäckiger Elemente erzwingen können.</span><span class="sxs-lookup"><span data-stu-id="1ec18-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="1ec18-109">PNP-Datei entfernen</span><span class="sxs-lookup"><span data-stu-id="1ec18-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="1ec18-110">PNP-Ordner entfernen</span><span class="sxs-lookup"><span data-stu-id="1ec18-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="1ec18-111">PNP-Listenelement entfernen</span><span class="sxs-lookup"><span data-stu-id="1ec18-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="1ec18-112">PNP-Liste entfernen</span><span class="sxs-lookup"><span data-stu-id="1ec18-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="1ec18-113">PNP-Feld entfernen (Spalte)</span><span class="sxs-lookup"><span data-stu-id="1ec18-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)