---
title: 932 aktualisieren AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289877"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="40f70-102">Upgrade von Azure Active Directory verbinden</span><span class="sxs-lookup"><span data-stu-id="40f70-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="40f70-p101">In der Standardeinstellung ist automatische Aktualisierung für Azure AD-Connect aktiviert wodurch sichergestellt, dass Sie die neueste Version ausgeführt werden. Um die automatischen Aktualisierung Einstellungen zu überprüfen, verwenden Sie das Cmdlet **Get-ADSyncAutoUpgrade** in Azure AD-PowerShell. Das Cmdlet gibt einen der folgenden Werte zurück:</span><span class="sxs-lookup"><span data-stu-id="40f70-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="40f70-106">**Aktiviert**: automatische Aktualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="40f70-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="40f70-107">**Deaktiviert**: automatische Aktualisierung ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="40f70-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="40f70-p102">**Angehalten**: das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten. Sie können diesen Wert nicht konfigurieren; Es wird vom System festgelegt.</span><span class="sxs-lookup"><span data-stu-id="40f70-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="40f70-110">Weitere Informationen finden Sie unter [Automatische Aktualisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="40f70-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="40f70-111">Informationen zum Herunterladen der neuesten Version von Azure Active Directory verbinden, wechseln Sie zur [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="40f70-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

