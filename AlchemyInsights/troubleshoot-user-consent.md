---
title: Problembehandlung bei der Zustimmung des Benutzers
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897721"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="aa9a1-102">Problembehandlung bei der Zustimmung des Benutzers</span><span class="sxs-lookup"><span data-stu-id="aa9a1-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="aa9a1-103">Sie können konfigurieren, wie Endbenutzer Anwendungen über das Azure Portal oder PowerShell zustimmen.</span><span class="sxs-lookup"><span data-stu-id="aa9a1-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="aa9a1-104">Weitere [Informationen finden Sie unter den Einstellungen für](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) die Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="aa9a1-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="aa9a1-105">Ein Administrator kann die [Microsoft Graph-API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) auch verwenden, um delegierten Berechtigungen im Namen eines einzelnen Benutzers seine Zustimmung zu erteilen.</span><span class="sxs-lookup"><span data-stu-id="aa9a1-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="aa9a1-106">Weitere Informationen finden Sie unter ["Zugriff im Auftrag eines Benutzers erhalten".](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="aa9a1-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="aa9a1-107">[Benutzer-Zustimmungsfehler:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)In diesem Artikel werden Fehler behandelt, die während des Prozesses der Zustimmung zu einer Anwendung auftreten können.</span><span class="sxs-lookup"><span data-stu-id="aa9a1-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="aa9a1-108">Wenn Sie unerwartete Zustimmungsaufforderungen beheben, die keine Fehlermeldungen enthalten, finden Sie weitere Informationen unter ["Authentifizierungsszenarien für Azure AD".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="aa9a1-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>