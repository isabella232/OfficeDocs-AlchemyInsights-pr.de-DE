---
title: Zugriffsüberprüfungen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013948"
---
# <a name="access-reviews"></a><span data-ttu-id="f3e37-102">Zugriffsüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="f3e37-102">Access reviews</span></span>

1. <span data-ttu-id="f3e37-103">**Aktivieren von Zugriffsüberprüfungen:** Sie können Rezensionen aktivieren, wenn Sie ein neues Zugriffspaket erstellen oder ein vorhandenes Zugriffspaket bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="f3e37-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="f3e37-104">[Erstellen einer Zugriffsüberprüfung eines Zugriffspakets in Azure AD-Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) beschreibt, wie Zugriffsüberprüfungen von Zugriffspaketen aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="f3e37-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="f3e37-105">**Zugriff überprüfen:** Azure AD-Berechtigungsverwaltung vereinfacht die Verwaltung des Zugriffs auf Gruppen, Anwendungen und SharePoint-Websites.</span><span class="sxs-lookup"><span data-stu-id="f3e37-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="f3e37-106">[Das Überprüfen des Zugriffs](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) auf ein Zugriffspaket in der Azure AD-Berechtigungsverwaltung beschreibt, wie Zugriffsüberprüfungen für andere Benutzer ausgeführt werden, die einem Zugriffspaket als festgelegter Prüfer zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="f3e37-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="f3e37-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span><span class="sxs-lookup"><span data-stu-id="f3e37-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="f3e37-108">In den meisten Fällen finden Endbenutzer eine Rezension, die ihre Antwort in **der Zugriffsteuerung aussteht.**</span><span class="sxs-lookup"><span data-stu-id="f3e37-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="f3e37-109">Dies gilt nur für Rezensionen von Gruppen und Anwendungen, nicht für Rollen.</span><span class="sxs-lookup"><span data-stu-id="f3e37-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="f3e37-110">Für alle Zugriffsüberprüfungen von Rollen müssen Endbenutzer zu Azure AD Privileged Identity Management (PIM) navigieren, um ihre Überprüfung abschließen zu können.</span><span class="sxs-lookup"><span data-stu-id="f3e37-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="f3e37-111">Anmelden beim Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="f3e37-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="f3e37-112">Navigieren Sie zu Azure AD PIM.</span><span class="sxs-lookup"><span data-stu-id="f3e37-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="f3e37-113">Wählen Sie im linken Navigationsbereich den Zugriff **"Aufgaben**  >  **überprüfen" aus.**</span><span class="sxs-lookup"><span data-stu-id="f3e37-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="f3e37-114">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="f3e37-114">For more information, see:</span></span>

- [<span data-ttu-id="f3e37-115">Durchführen einer Zugriffsüberprüfung meiner Azure AD-Verzeichnisrollen in PIM </span><span class="sxs-lookup"><span data-stu-id="f3e37-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="f3e37-116">Durchführen einer Zugriffsüberprüfung meiner Azure-Ressourcenrollen in PIM</span><span class="sxs-lookup"><span data-stu-id="f3e37-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)