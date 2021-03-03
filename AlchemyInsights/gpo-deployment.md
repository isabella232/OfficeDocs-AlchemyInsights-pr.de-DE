---
title: GPO-Bereitstellung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417011"
---
# <a name="gpo-deployment"></a><span data-ttu-id="ace5a-102">GPO-Bereitstellung</span><span class="sxs-lookup"><span data-stu-id="ace5a-102">GPO Deployment</span></span>

<span data-ttu-id="ace5a-103">Einstellungen für Benutzer- und Computerobjekte in Azure Active Directory Domain Services (Azure AD DS) werden häufig mit Gruppenrichtlinienobjekten (GPOs) verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ace5a-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="ace5a-104">Azure AD DS enthält integrierte GPOs für die Container "AADDC-Benutzer" und "AADDC-Computer".</span><span class="sxs-lookup"><span data-stu-id="ace5a-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="ace5a-105">Sie können diese integrierten Gruppenrichtlinienobjekte anpassen, um Gruppenrichtlinien nach Bedarf für Ihre Umgebung zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="ace5a-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="ace5a-106">Mitglieder der Gruppe der Azure AD DC-Administratoren verfügen in der Azure AD DS-Domäne über Administratorrechte für Gruppenrichtlinien und können auch benutzerdefinierte Gruppenrichtlinienobjekte und Organisationseinheiten erstellen.</span><span class="sxs-lookup"><span data-stu-id="ace5a-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="ace5a-107">Weitere Informationen dazu, was Gruppenrichtlinien sind und wie sie funktioniert, finden Sie unter [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="ace5a-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="ace5a-108">In einer Hybridumgebung werden in einer lokalen AD DS-Umgebung konfigurierte Gruppenrichtlinien nicht mit Azure AD DS synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="ace5a-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="ace5a-109">Um Konfigurationseinstellungen für Benutzer oder Computer in Azure AD DS zu definieren, bearbeiten Sie eines der Standardrichtlinienobjekte, oder erstellen Sie ein benutzerdefiniertes Gruppenrichtlinienobjekt.</span><span class="sxs-lookup"><span data-stu-id="ace5a-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="ace5a-110">In diesem Artikel, [Verwalten von Gruppenrichtlinienrichtlinien](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) wird gezeigt, wie Sie die Tools für die Gruppenrichtlinienverwaltung installieren, die integrierten Gruppenrichtlinienobjekte bearbeiten und wie benutzerdefinierte Gruppenrichtlinienobjekte erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="ace5a-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
