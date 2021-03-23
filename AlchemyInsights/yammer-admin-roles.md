---
title: Informationen Yammer Administratoren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995261"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="bb66f-102">Informationen Yammer Administratoren</span><span class="sxs-lookup"><span data-stu-id="bb66f-102">About Yammer admins</span></span>

<span data-ttu-id="bb66f-103">**Netzwerkadministratoren**</span><span class="sxs-lookup"><span data-stu-id="bb66f-103">**Network admins**</span></span>

<span data-ttu-id="bb66f-104">Globale Administratoren werden automatisch in die Rolle "Überprüfter Administrator" in einem Yammer heraufgestuft.</span><span class="sxs-lookup"><span data-stu-id="bb66f-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="bb66f-105">In den folgenden Fällen tritt diese Aktion möglicherweise nicht ordnungsgemäß auf:</span><span class="sxs-lookup"><span data-stu-id="bb66f-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="bb66f-106">Mehrere Yammer vorhanden, und der Administrator wird bei der falschen angemeldet.</span><span class="sxs-lookup"><span data-stu-id="bb66f-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="bb66f-107">[Die Netzwerkkonsolidierung](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ist erforderlich, um zu einem Yammer zu kommen.</span><span class="sxs-lookup"><span data-stu-id="bb66f-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="bb66f-108">Azure PIM wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="bb66f-108">Azure PIM is being used.</span></span> <span data-ttu-id="bb66f-109">Der Benutzer wird möglicherweise nicht lange genug zum globalen Administrator heraufgestuft, damit die Heraufstufung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="bb66f-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="bb66f-110">Ein zukünftiges Update für Yammer kann dieses Problem beheben, es ist jedoch am besten, Benutzer manuell zum globalen Administrator zu bewerben.</span><span class="sxs-lookup"><span data-stu-id="bb66f-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="bb66f-111">Es liegt ein Synchronisierungsproblem mit dem Yammer vor.</span><span class="sxs-lookup"><span data-stu-id="bb66f-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="bb66f-112">In diesem Fall ist eine Supportanfrage für weitere Untersuchungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb66f-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="bb66f-113">Weitere Informationen zu Yammer Administratorrollen finden Sie unter [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="bb66f-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="bb66f-114">**Gruppenadministratoren**</span><span class="sxs-lookup"><span data-stu-id="bb66f-114">**Group admins**</span></span>

<span data-ttu-id="bb66f-115">Gruppenadministratoren für mit Microsoft 365 verbundene Gruppen werden mit der Gruppenmitgliedschaft aus Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bb66f-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="bb66f-116">Bei großen Gruppen kann diese Synchronisierung einen längeren Zeitraum dauern.</span><span class="sxs-lookup"><span data-stu-id="bb66f-116">For large groups, this sync can take an extended period.</span></span>
