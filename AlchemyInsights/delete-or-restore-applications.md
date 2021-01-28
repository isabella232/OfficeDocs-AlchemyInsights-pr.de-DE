---
title: Löschen oder Wiederherstellen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013957"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="dcb73-102">Löschen oder Wiederherstellen von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="dcb73-102">Delete or restore applications</span></span>

<span data-ttu-id="dcb73-103">**So löschen Sie eine Anwendung aus Ihrem Azure AD-Mandanten:**</span><span class="sxs-lookup"><span data-stu-id="dcb73-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="dcb73-104">Wählen Sie **im Azure AD-Portal** **Enterprise-Anwendungen aus.**</span><span class="sxs-lookup"><span data-stu-id="dcb73-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="dcb73-105">Suchen Und wählen Sie dann die Anwendung aus, die Sie löschen möchten.</span><span class="sxs-lookup"><span data-stu-id="dcb73-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="dcb73-106">Wählen Sie **im Abschnitt "Verwalten"** im linken Bereich **"Eigenschaften" aus.**</span><span class="sxs-lookup"><span data-stu-id="dcb73-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="dcb73-107">Wählen **Sie "Löschen"** und dann **"Ja"** aus, um zu bestätigen, dass Sie die App aus Ihrem Azure AD-Mandanten löschen möchten.</span><span class="sxs-lookup"><span data-stu-id="dcb73-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="dcb73-108">Weitere Informationen zum Löschen einer App finden Sie unter Schnellstart: Löschen einer Anwendung aus Ihrem [Azure Active Directory (Azure AD)-Mandanten.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="dcb73-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="dcb73-109">In PowerShell entfernt das [Cmdlet "Remove-AzureADApplicationProxyApplication" Anwendungsproxykonfigurationen](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) aus einer bestimmten Anwendung in Azure Active Directory und kann die Anwendung vollständig löschen, falls angegeben.</span><span class="sxs-lookup"><span data-stu-id="dcb73-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="dcb73-110">Sie können **eine gelöschte Anwendung mithilfe** von PowerShell wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="dcb73-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="dcb73-111">Nachdem die wiederherzustellende Anwendung identifiziert wurde, können Sie sie mithilfe von [Restore-AzureADDeletedApplication wiederherstellen.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)</span><span class="sxs-lookup"><span data-stu-id="dcb73-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
