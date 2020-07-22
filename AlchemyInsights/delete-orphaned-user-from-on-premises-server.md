---
title: Verwaiste Benutzer vom lokalen Server löschen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186132"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="caa55-102">Verwaiste Benutzer vom lokalen Server löschen</span><span class="sxs-lookup"><span data-stu-id="caa55-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="caa55-103">Führen Sie die folgenden Schritte aus, um einen verwaisten Benutzer zu entfernen:</span><span class="sxs-lookup"><span data-stu-id="caa55-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="caa55-104">Erzwingen Sie die Verzeichnissynchronisierung, indem Sie die Anweisungen in [Was bedeutet Hybrididentität in Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories) befolgen.</span><span class="sxs-lookup"><span data-stu-id="caa55-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="caa55-105">Um die Verzeichnissynchronisierung zu verifizieren, siehe [Was bedeutet Hybrididentität in Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="caa55-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="caa55-106">Wenn die Synchronisierung ordnungsgemäß funktioniert, das Löschen des Active Directory-Objekts jedoch noch nicht an Azure AD weitergegeben wird, können Sie das verwaiste Objekt mithilfe eines der folgenden Azure Active Directory-Module für Windows PowerShell-Cmdlets manuell entfernen:</span><span class="sxs-lookup"><span data-stu-id="caa55-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="caa55-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="caa55-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="caa55-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="caa55-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="caa55-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="caa55-109">Remove-MsolUser</span></span>

    <span data-ttu-id="caa55-110">Wenn Sie beispielsweise die verwaiste Benutzer-ID manuell entfernen möchten, die john.smith@contoso.com ursprünglich mithilfe der Verzeichnissynchronisierung erstellt wurde, führen Sie das folgende Cmdlet aus:</span><span class="sxs-lookup"><span data-stu-id="caa55-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="caa55-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="caa55-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>