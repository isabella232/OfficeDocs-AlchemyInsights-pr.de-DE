---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507414"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="3d203-102">Synchronisierungsfehler aufgrund doppelter Objekte</span><span class="sxs-lookup"><span data-stu-id="3d203-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="3d203-103">Möglicherweise wird eine der folgenden Fehlermeldungen angezeigt, wenn die Verzeichnissynchronisierung in Office 365 abgeschlossen wird:</span><span class="sxs-lookup"><span data-stu-id="3d203-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="3d203-104">Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="3d203-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="3d203-105">In Ihrem Microsoft Online Services-Verzeichnis ist bereits ein synchronisiertes Objekt mit derselben Proxyadresse vorhanden.</span><span class="sxs-lookup"><span data-stu-id="3d203-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="3d203-106">Dieses Objekt kann nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: userPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3d203-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="3d203-107">Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix Dirsync-Tool zur Fehlerbehebung](https://www.microsoft.com/download/details.aspx?id=36832)herunter, und führen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="3d203-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="3d203-108">Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="3d203-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
