---
title: Verwenden von PowerShell für Freigaberichtlinien und Organisationsbeziehungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 378dedb332ced2c86899401c54726eb6b7e25d08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773414"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="07c1e-102">Verwenden von PowerShell für Freigaberichtlinien und Organisationsbeziehungen</span><span class="sxs-lookup"><span data-stu-id="07c1e-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="07c1e-103">Informationen zu Organisationsbeziehungen finden Sie in den detaillierten Syntax- und Parameterinformationen für: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) UND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="07c1e-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="07c1e-104">Zum Erstellen einer Freigaberichtlinie verwenden Sie [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="07c1e-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="07c1e-105">Um [eine Freigaberichtlinie auf ein Postfach oder einen Benutzer anzuwenden](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), müssen Sie eine Kombination aus [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) und [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) mit der neu erstellten Richtlinie verwenden.</span><span class="sxs-lookup"><span data-stu-id="07c1e-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="07c1e-106">Zum [Ändern, Deaktivieren oder Entfernen einer Freigaberichtlinie](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) müssen Sie [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) verwenden.</span><span class="sxs-lookup"><span data-stu-id="07c1e-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="07c1e-107">**Für vollständige Informationen zu diesem Thema lesen Sie:**</span><span class="sxs-lookup"><span data-stu-id="07c1e-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="07c1e-108">Freigabe in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="07c1e-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)