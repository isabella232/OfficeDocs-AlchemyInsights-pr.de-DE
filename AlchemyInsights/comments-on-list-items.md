---
title: Kommentare zu Listenelementen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947508"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="6d311-102">Kommentare zu Listenelementen</span><span class="sxs-lookup"><span data-stu-id="6d311-102">Comments on List items</span></span>

<span data-ttu-id="6d311-103">Benutzer werden in Kürze Kommentare zu Listenelementen hinzufügen und löschen können.</span><span class="sxs-lookup"><span data-stu-id="6d311-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="6d311-104">Benutzer können alle Kommentare zu einem Listenelement anzeigen und zwischen Ansichten filtern, die Kommentare oder Aktivitäten im Zusammenhang mit einem Element anzeigen.</span><span class="sxs-lookup"><span data-stu-id="6d311-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="6d311-105">**Timing** :</span><span class="sxs-lookup"><span data-stu-id="6d311-105">**Timing** :</span></span>

<span data-ttu-id="6d311-106">**Targeted Release** : schrittweiser Rollout Mitte Oktober und voraussichtlich bis Mitte November abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="6d311-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="6d311-107">**Standard Version** : schrittweiser Rollout Mitte November und voraussichtlich bis Anfang Dezember abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="6d311-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="6d311-108">**Rollout** : gezielte Freigabe für die gesamte Organisation</span><span class="sxs-lookup"><span data-stu-id="6d311-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="6d311-109">Benutzer müssen Folgendes beachten, bevor Sie Kommentare hinzufügen und löschen können:</span><span class="sxs-lookup"><span data-stu-id="6d311-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="6d311-110">Kommentare entsprechen den Berechtigungseinstellungen von SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6d311-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="6d311-111">Klassische Listen, die noch nicht für die Darstellung in modernen Benutzeroberflächen wie Aufgabenlisten erstellt wurden, verfügen nicht über diese Kommentarfunktion.</span><span class="sxs-lookup"><span data-stu-id="6d311-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="6d311-112">Das Kommentieren von Listen in Microsoft Teams steht in dieser Version nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="6d311-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="6d311-113">Kommentare werden nicht durch die Suche indiziert.</span><span class="sxs-lookup"><span data-stu-id="6d311-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="6d311-114">Administratoren können dieses Feature auf Organisationsebene deaktivieren, indem Sie den Parameter **CommentsOnListItemsDisabled** im PowerShell-Cmdlet " **Sets-SPOTenant** " ändern.</span><span class="sxs-lookup"><span data-stu-id="6d311-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="6d311-115">Es ist derzeit nicht möglich, das kommentieren auf Website-oder Listenebene zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="6d311-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="6d311-116">Wir hoffen, diese Steuerelemente in einem späteren Update zu haben, wahrscheinlich im ersten Quartal 2021.</span><span class="sxs-lookup"><span data-stu-id="6d311-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
