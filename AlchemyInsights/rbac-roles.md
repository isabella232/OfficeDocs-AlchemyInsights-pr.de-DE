---
title: 'RBAC-Rollen '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576526"
---
# <a name="rbac-rules"></a><span data-ttu-id="d78ca-102">RBAC-Regeln</span><span class="sxs-lookup"><span data-stu-id="d78ca-102">RBAC rules</span></span>

<span data-ttu-id="d78ca-103">Wenn Sie den Berechtigungsfehler erhalten:</span><span class="sxs-lookup"><span data-stu-id="d78ca-103">If you get the permission error:</span></span> 

- <span data-ttu-id="d78ca-104">**Der Client mit Objekt-ID verfügt nicht über die Berechtigung zum Ausführen einer Aktion über den Bereich (Code: AuthorizationFailed)**: Wenn Sie versuchen, eine Ressource zu erstellen, überprüfen Sie, ob Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über Schreibberechtigungen für die Ressource im ausgewählten Bereich verfügt.</span><span class="sxs-lookup"><span data-stu-id="d78ca-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="d78ca-105">Um beispielsweise virtuelle Computer in einer Ressourcengruppe zu verwalten, sollten Sie über die Rolle " [beteiligte virtuelle Computer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) " für die Ressourcengruppe (oder übergeordneter Bereich) verfügen.</span><span class="sxs-lookup"><span data-stu-id="d78ca-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="d78ca-106">Eine Liste der Berechtigungen für jede integrierte Rolle finden Sie unter [integrierte Rollen für Azure-Ressourcen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d78ca-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="d78ca-107">**Sie verfügen nicht über die Berechtigung zum Erstellen einer Supportanforderung**: Wenn Sie versuchen, ein Support Ticket zu erstellen oder zu aktualisieren, stellen Sie sicher, dass Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über die Microsoft. Support/supportTickets/Write-Berechtigung verfügt, beispielsweise den [Mitwirkenden für Supportanfragen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="d78ca-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="d78ca-108">Es **können keine weiteren Rollenzuweisungen erstellt werden (Code: RoleAssignmentLimitExceeded)**: Wenn Sie versuchen, eine Rolle zuzuweisen, versuchen Sie, die Anzahl der Rollenzuweisungen zu verringern, indem Sie stattdessen Rollen zu Gruppen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="d78ca-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="d78ca-109">Azure unterstützt bis zu **2000** Rollenzuweisungen pro Abonnement.</span><span class="sxs-lookup"><span data-stu-id="d78ca-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="d78ca-110">Weitere Informationen zu Azure-RBAC-Rollen finden Sie unter [Azure RBAC Roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d78ca-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
