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
# <a name="rbac-rules"></a>RBAC-Regeln

Wenn Sie den Berechtigungsfehler erhalten: 

- **Der Client mit Objekt-ID verfügt nicht über die Berechtigung zum Ausführen einer Aktion über den Bereich (Code: AuthorizationFailed)**: Wenn Sie versuchen, eine Ressource zu erstellen, überprüfen Sie, ob Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über Schreibberechtigungen für die Ressource im ausgewählten Bereich verfügt. Um beispielsweise virtuelle Computer in einer Ressourcengruppe zu verwalten, sollten Sie über die Rolle " [beteiligte virtuelle Computer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) " für die Ressourcengruppe (oder übergeordneter Bereich) verfügen. Eine Liste der Berechtigungen für jede integrierte Rolle finden Sie unter [integrierte Rollen für Azure-Ressourcen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Sie verfügen nicht über die Berechtigung zum Erstellen einer Supportanforderung**: Wenn Sie versuchen, ein Support Ticket zu erstellen oder zu aktualisieren, stellen Sie sicher, dass Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über die Microsoft. Support/supportTickets/Write-Berechtigung verfügt, beispielsweise den [Mitwirkenden für Supportanfragen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Es **können keine weiteren Rollenzuweisungen erstellt werden (Code: RoleAssignmentLimitExceeded)**: Wenn Sie versuchen, eine Rolle zuzuweisen, versuchen Sie, die Anzahl der Rollenzuweisungen zu verringern, indem Sie stattdessen Rollen zu Gruppen zuweisen. Azure unterstützt bis zu **2000** Rollenzuweisungen pro Abonnement.

Weitere Informationen zu Azure-RBAC-Rollen finden Sie unter [Azure RBAC Roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
