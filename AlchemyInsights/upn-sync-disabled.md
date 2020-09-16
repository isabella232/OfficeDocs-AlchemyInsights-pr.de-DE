---
title: UPN-Synchronisierung deaktiviert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749513"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="d80e1-102">UPN-Synchronisierung deaktiviert</span><span class="sxs-lookup"><span data-stu-id="d80e1-102">UPN sync disabled</span></span>

<span data-ttu-id="d80e1-103">Wenn Sie mit der Synchronisierung mit Azure AD vor dem 30. März 2016 begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um UPN Soft Match nur für Ihre Organisation zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="d80e1-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="d80e1-104">**Festlegen-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $true**</span><span class="sxs-lookup"><span data-stu-id="d80e1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="d80e1-105">UPN Soft Match wird automatisch für Organisationen aktiviert, die mit der Synchronisierung mit Azure AD begonnen haben oder nach dem 30. März 2016.</span><span class="sxs-lookup"><span data-stu-id="d80e1-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="d80e1-106">Weitere Informationen zum Aktivieren von Soft Match unter UPN und anderen Synchronisierungsfeatures finden Sie unter [Azure AD Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="d80e1-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

