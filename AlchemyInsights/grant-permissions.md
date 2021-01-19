---
title: Erteilen von Berechtigungen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897720"
---
# <a name="grant-permissions"></a><span data-ttu-id="de946-102">Erteilen von Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de946-102">Grant permissions</span></span>

1. <span data-ttu-id="de946-103">Gewähren der mandantenweiten Administratorzuseignung: Unter "Mandantenweite Administratorzuwilligung für eine Anwendung erteilen" finden Sie schrittweise Anleitungen zum Erteilen der mandantenweiten Administratorzusendung aus dem Azure-Portal, mithilfe von Azure AD PowerShell oder aus der Zustimmungsaufforderung selbst.  [](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="de946-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="de946-104">**Erteilen der** Zustimmung im Namen eines bestimmten Benutzers: Anstatt die Zustimmung für die gesamte Organisation zu erteilen, kann ein Administrator auch die [Microsoft Graph-API](https://docs.microsoft.com/graph/use-the-api) verwenden, um delegierte Berechtigungen im Namen eines einzelnen Benutzers zu erteilen.</span><span class="sxs-lookup"><span data-stu-id="de946-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="de946-105">Weitere Informationen finden Sie unter ["Zugriff im Auftrag eines Benutzers erhalten".](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="de946-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>