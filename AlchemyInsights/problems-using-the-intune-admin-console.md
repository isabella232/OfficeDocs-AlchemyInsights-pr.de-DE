---
title: Probleme beim Verwenden der Intune-Verwaltungskonsole
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46523018"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="66dc4-102">Probleme beim Verwenden der Intune-Verwaltungskonsole</span><span class="sxs-lookup"><span data-stu-id="66dc4-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="66dc4-103">**"Zugriff verweigert" beim Navigieren im Intune-Verwaltungsportal.**</span><span class="sxs-lookup"><span data-stu-id="66dc4-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="66dc4-104">Wenn Sie Mitglied einer benutzerdefinierten Intune-Rolle sind, stellen Sie sicher, dass Ihrem Konto eine Intune- oder Enterprise Mobility Suite-Lizenz zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="66dc4-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="66dc4-105">Wenn Sie Configuration Manager zum Verwalten von Geräten verwenden, stellen Sie sicher, dass Sie nicht zur Intune-Benutzersammlung für Configuration Manager-MDM gehören.</span><span class="sxs-lookup"><span data-stu-id="66dc4-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="66dc4-106">Stellen Sie sicher, dass Ihnen im Blatt"Intune-Rolle" die entsprechenden RBAC-Berechtigungen (rollenbasierte Zugriffssteuerung) zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="66dc4-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="66dc4-107">Vergewissern Sie sich, dass die verwendete Gruppe keine Verteilerliste ist.</span><span class="sxs-lookup"><span data-stu-id="66dc4-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="66dc4-108">Intune im Azure-Portal unterstützt nur Benutzerkonten, die zu Azure Active Directory-Sicherheitsgruppen gehören.</span><span class="sxs-lookup"><span data-stu-id="66dc4-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="66dc4-109">Überprüfen Sie Ihre Gruppen unter Azure-Portal > **Intune** > **Gruppen**, oder unter Azure-Portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="66dc4-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="66dc4-110">**Der Benutzer verfügt über zu viele Berechtigungen für die zugewiesene Intune-Rolle**</span><span class="sxs-lookup"><span data-stu-id="66dc4-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="66dc4-111">Weisen Sie den Benutzer an, zu **Intune** > **Intune-Rollen** > **Meine Berechtigungen** > **Exportieren** zu wechseln, um die gewährten Berechtigungen zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="66dc4-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="66dc4-112">**Ich habe eine Bereichsgruppe zu einer Rolle hinzugefügt, aber die Benutzer in dieser Rolle sehen weiterhin andere Benutzer oder Geräte.**</span><span class="sxs-lookup"><span data-stu-id="66dc4-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="66dc4-113">Bereichsgruppen filtern keine Benutzer oder Geräte heraus.</span><span class="sxs-lookup"><span data-stu-id="66dc4-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="66dc4-114">Bereichsgruppen:</span><span class="sxs-lookup"><span data-stu-id="66dc4-114">Scope groups:</span></span>

- <span data-ttu-id="66dc4-115">Beschränken, web Benutzer Richtlinien oder Anwendungen zuordnen können.</span><span class="sxs-lookup"><span data-stu-id="66dc4-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="66dc4-116">Erlauben nur bestimmten Benutzern das Ausführen von Remoteaufgaben auf Geräten.</span><span class="sxs-lookup"><span data-stu-id="66dc4-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="66dc4-117">Weitere Informationen über Bereichsgruppen finden Sie unter [Rollenbasierte Zugriffssteuerung (RBAC) mit Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="66dc4-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="66dc4-118">**Ich habe einen Benutzer zu einer Intune-Rolle hinzugefügt, aber er hat immer noch vollen Zugriff auf die Intune-Verwaltungskonsole.**</span><span class="sxs-lookup"><span data-stu-id="66dc4-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="66dc4-119">Navigieren Sie im Azure-Portal zu Intune > **Benutzer**dem Benutzer keine der folgenden Rollen im Azure-Portal zugewiesen ist:</span><span class="sxs-lookup"><span data-stu-id="66dc4-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="66dc4-120">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="66dc4-120">Global administrator</span></span>
- <span data-ttu-id="66dc4-121">Intune-Dienstadministrator</span><span class="sxs-lookup"><span data-stu-id="66dc4-121">Intune service administrator</span></span>
- <span data-ttu-id="66dc4-122">SharePoint-Administrator</span><span class="sxs-lookup"><span data-stu-id="66dc4-122">SharePoint administrator</span></span>

<span data-ttu-id="66dc4-123">Weitere Informationen finden Sie unter [Rollenbasierte Zugriffssteuerung (RBAC) mit Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="66dc4-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="66dc4-124">**Access-Probleme**</span><span class="sxs-lookup"><span data-stu-id="66dc4-124">**Access Issues**</span></span>

<span data-ttu-id="66dc4-125">Weitere Informationen finden Sie unter [Anmelden bei Office 365, Azure oder Intune nicht möglich](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="66dc4-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>