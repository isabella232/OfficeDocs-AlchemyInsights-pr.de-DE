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
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532330"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="97c4f-102">UPN-Synchronisierung deaktiviert</span><span class="sxs-lookup"><span data-stu-id="97c4f-102">UPN sync disabled</span></span>

<span data-ttu-id="97c4f-103">Wenn Sie mit der Synchronisierung mit Azure AD vor dem 30. März 2016 begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um UPN Soft Match nur für Ihre Organisation zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="97c4f-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="97c4f-104">**Festlegen-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $true**</span><span class="sxs-lookup"><span data-stu-id="97c4f-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="97c4f-105">UPN Soft Match wird automatisch für Organisationen aktiviert, die mit der Synchronisierung mit Azure AD begonnen haben oder nach dem 30. März 2016.</span><span class="sxs-lookup"><span data-stu-id="97c4f-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="97c4f-106">Weitere Informationen zum Aktivieren von Soft Match unter UPN und anderen Synchronisierungsfeatures finden Sie unter [Azure AD Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="97c4f-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

