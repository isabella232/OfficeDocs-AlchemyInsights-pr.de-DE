---
title: Gruppensynchronisierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243904"
---
# <a name="group-sync"></a><span data-ttu-id="6d3ba-102">Gruppensynchronisierung</span><span class="sxs-lookup"><span data-stu-id="6d3ba-102">Group sync</span></span>

<span data-ttu-id="6d3ba-103">Dieser Artikel enthält Anleitungen zur Gruppensynchronisierung.</span><span class="sxs-lookup"><span data-stu-id="6d3ba-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="6d3ba-104">Wenn ein globaler Administrator oder Gruppenbesitzer nicht in der Lage ist, Gruppeneigenschaften zu ändern oder Mitglieder hinzuzufügen oder Besitzer im Azure-Portal zuzuweisen, stellen Sie sicher, dass die Quelle der Berechtigung für die Gruppe Azure Active Directory (Azure AD) ist, damit der globale Administrator oder Gruppenbesitzer die Gruppe ändern kann.</span><span class="sxs-lookup"><span data-stu-id="6d3ba-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="6d3ba-105">Bevor Sie versuchen, eine synchronisierte Gruppe in Azure AD zu löschen, stellen Sie sicher, dass Sie [alle zugewiesenen Lizenzen gelöscht haben](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced), um Fehler zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="6d3ba-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="6d3ba-106">Informationen zum Synchronisieren von Benutzern, Gruppen und Kontakten finden Sie unter [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts). Folgen Sie [Synchronisieren einer lokalen Gruppe mit Azure mithilfe von Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) , um lokalen Gruppen mithilfe von AD Connect zu synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="6d3ba-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="6d3ba-107">Befolgen Sie dieses Handbuch [Problembehandlung bei Fehlern während der Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors), um häufige Fehler während der Synchronisierung zu beheben.</span><span class="sxs-lookup"><span data-stu-id="6d3ba-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

