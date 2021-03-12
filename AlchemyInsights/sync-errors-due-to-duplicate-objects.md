---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708061"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a2ecf-102">Synchronisierungsfehler aufgrund doppelter Objekte</span><span class="sxs-lookup"><span data-stu-id="a2ecf-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a2ecf-103">Möglicherweise erhalten Sie eine der folgenden Fehlermeldungen, wenn die Verzeichnissynchronisierung in Microsoft 365 abgeschlossen ist:</span><span class="sxs-lookup"><span data-stu-id="a2ecf-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="a2ecf-104">Dieses Objekt kann nicht Microsoft Online Services aktualisiert werden, da die folgenden diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt im lokalen Verzeichnis zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="a2ecf-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="a2ecf-105">Ein synchronisiertes Objekt mit derselben Proxyadresse ist bereits in Ihrem Microsoft Online Services vorhanden.</span><span class="sxs-lookup"><span data-stu-id="a2ecf-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="a2ecf-106">Dieses Objekt kann nicht aktualisiert werden, da die folgenden Diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a2ecf-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="a2ecf-107">Laden Sie das [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix)herunter, und führen Sie es aus, um das Problem zu identifizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="a2ecf-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="a2ecf-108">Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a2ecf-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
