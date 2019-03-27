---
title: UPN-Synchronisierung deaktiviert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767227"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="45669-102">UPN-Synchronisierung deaktiviert</span><span class="sxs-lookup"><span data-stu-id="45669-102">UPN sync disabled</span></span>

<span data-ttu-id="45669-103">Wenn Sie vor dem 30. März 2016 mit der Synchronisierung mit Azure AD begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um die UPN-weiche Übereinstimmung nur für Ihre Organisation zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="45669-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="45669-104">**Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $True**</span><span class="sxs-lookup"><span data-stu-id="45669-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="45669-105">Die UPN-weiche Übereinstimmung wird automatisch für Organisationen aktiviert, die an oder nach dem 30. März 2016 mit Azure AD synchronisiert haben.</span><span class="sxs-lookup"><span data-stu-id="45669-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="45669-106">Weitere Informationen zum Aktivieren von Soft Match für UPN und andere Synchronisierungsfunktionen finden Sie unter [Azure AD Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="45669-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

