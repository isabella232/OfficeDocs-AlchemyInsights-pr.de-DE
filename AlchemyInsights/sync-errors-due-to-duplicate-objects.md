---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767126"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="4ca28-102">Synchronisierungsfehler aufgrund doppelter Objekte</span><span class="sxs-lookup"><span data-stu-id="4ca28-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="4ca28-103">Wenn die Verzeichnissynchronisierung in Microsoft 365 abgeschlossen ist, wird möglicherweise eine der folgenden Fehlermeldungen angezeigt:</span><span class="sxs-lookup"><span data-stu-id="4ca28-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="4ca28-104">Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="4ca28-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="4ca28-105">In Ihrem Microsoft Online Services-Verzeichnis ist bereits ein synchronisiertes Objekt mit derselben Proxyadresse vorhanden.</span><span class="sxs-lookup"><span data-stu-id="4ca28-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="4ca28-106">Dieses Objekt kann nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: userPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4ca28-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="4ca28-107">Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix Dirsync-Tool zur Fehlerbehebung](https://www.microsoft.com/download/details.aspx?id=36832)herunter, und führen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="4ca28-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="4ca28-108">Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="4ca28-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
