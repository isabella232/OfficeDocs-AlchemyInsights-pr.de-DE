---
title: Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719664"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="996d9-102">Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt</span><span class="sxs-lookup"><span data-stu-id="996d9-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="996d9-103">Der Benutzer gehört möglicherweise zu einer Rolle, die nicht über den richtigen AppsForOfficeEnabled-Parameter verfügt.</span><span class="sxs-lookup"><span data-stu-id="996d9-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="996d9-104">Führen Sie dieses Cmdlet aus, um zu ermitteln, ob dem Benutzer die richtige Rolle zugeordnet ist:</span><span class="sxs-lookup"><span data-stu-id="996d9-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="996d9-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="996d9-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="996d9-106">Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="996d9-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
