---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781261"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="3f0a8-102">Synchronisierungsfehler aufgrund doppelter Objekte</span><span class="sxs-lookup"><span data-stu-id="3f0a8-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="3f0a8-103">Wenn die Verzeichnissynchronisierung abgeschlossen ist, wird möglicherweise eine der folgenden Fehlermeldungen angezeigt:</span><span class="sxs-lookup"><span data-stu-id="3f0a8-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="3f0a8-104">Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden Attribute, die diesem Objekt zugeordnet sind, Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="3f0a8-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="3f0a8-105">Ein synchronisiertes Objekt mit derselben Proxyadresse ist bereits in Ihrem Microsoft Online Services-Verzeichnis vorhanden.</span><span class="sxs-lookup"><span data-stu-id="3f0a8-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="3f0a8-106">Dieses Objekt kann nicht aktualisiert werden, da die folgenden Attribute, die diesem Objekt zugeordnet sind, Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnisdienste zugeordnet sind: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3f0a8-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="3f0a8-107">Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix Dirsync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832)herunter und führen es aus.</span><span class="sxs-lookup"><span data-stu-id="3f0a8-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="3f0a8-108">Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="3f0a8-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

