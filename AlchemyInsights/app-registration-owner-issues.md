---
title: Probleme mit dem Besitzer der App-Registrierung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123113"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="99573-102">Probleme mit dem Besitzer der App-Registrierung</span><span class="sxs-lookup"><span data-stu-id="99573-102">App Registration Owner issues</span></span>

<span data-ttu-id="99573-103">Im Folgenden sind die verfügbaren Methoden zum Hinzufügen von Prinzipale als Besitzer für App-Registrierungen verfügbar:</span><span class="sxs-lookup"><span data-stu-id="99573-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="99573-104">Verwenden des Azure AD PowerShell-Moduls –</span><span class="sxs-lookup"><span data-stu-id="99573-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="99573-105">Referenz: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="99573-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="99573-106">Verwenden von Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="99573-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="99573-107">Referenz: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="99573-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="99573-108">Verwenden von MS Graph –</span><span class="sxs-lookup"><span data-stu-id="99573-108">Using MS Graph -</span></span>

    <span data-ttu-id="99573-109">Referenz: [Besitzer hinzufügen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="99573-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="99573-110">Verwenden des Azure AD-Portals – Navigieren Sie zu [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App-Registrierung > Wählen Sie Ihre Anwendung > Besitzer > Hinzufügen von Besitzern</span><span class="sxs-lookup"><span data-stu-id="99573-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="99573-111">**Sie können Ihre Anwendung nicht auf dem Blatt App-Registrierungen anzeigen, obwohl Sie der Besitzer dieser Anwendung sind?**</span><span class="sxs-lookup"><span data-stu-id="99573-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="99573-112">Der Besitzer einer App ist keine Administratorrolle.</span><span class="sxs-lookup"><span data-stu-id="99573-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="99573-113">Wenn die Einstellung [Zugriff auf Azure AD-Verwaltungsportal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) einschränken aktiviert ist, kann nur der Administrator die Anwendungen im App-Registrierungsportal anzeigen.</span><span class="sxs-lookup"><span data-stu-id="99573-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="99573-114">Damit ein Besitzer die Anwendungen anzeigen kann, deaktivieren Sie diese Einstellung (Legen Sie dies auf NEIN) oder weisen Sie dem Besitzer nur für die bestimmte Anwendung administratorrolle zu.</span><span class="sxs-lookup"><span data-stu-id="99573-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="99573-115">Dafür benötigen Sie jedoch eine Azure AD Premium P2-Lizenz und aktivieren [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span><span class="sxs-lookup"><span data-stu-id="99573-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
