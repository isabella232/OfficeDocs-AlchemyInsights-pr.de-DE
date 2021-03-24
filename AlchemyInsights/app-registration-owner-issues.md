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
# <a name="app-registration-owner-issues"></a>Probleme mit dem Besitzer der App-Registrierung

Im Folgenden sind die verfügbaren Methoden zum Hinzufügen von Prinzipale als Besitzer für App-Registrierungen verfügbar:

- Verwenden des Azure AD PowerShell-Moduls –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referenz: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Verwenden von Azure CLI – `az ad app owner add`

    Referenz: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Verwenden von MS Graph –

    Referenz: [Besitzer hinzufügen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Verwenden des Azure AD-Portals – Navigieren Sie zu [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App-Registrierung > Wählen Sie Ihre Anwendung > Besitzer > Hinzufügen von Besitzern

**Sie können Ihre Anwendung nicht auf dem Blatt App-Registrierungen anzeigen, obwohl Sie der Besitzer dieser Anwendung sind?**

Der Besitzer einer App ist keine Administratorrolle. Wenn die Einstellung [Zugriff auf Azure AD-Verwaltungsportal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) einschränken aktiviert ist, kann nur der Administrator die Anwendungen im App-Registrierungsportal anzeigen. Damit ein Besitzer die Anwendungen anzeigen kann, deaktivieren Sie diese Einstellung (Legen Sie dies auf NEIN) oder weisen Sie dem Besitzer nur für die bestimmte Anwendung administratorrolle zu. Dafür benötigen Sie jedoch eine Azure AD Premium P2-Lizenz und aktivieren [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
