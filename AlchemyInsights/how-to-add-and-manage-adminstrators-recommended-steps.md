---
title: Hinzufügen und Verwalten von Administratoren – empfohlene Schritte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755834"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="05976-102">Hinzufügen und Verwalten von Administratoren – empfohlene Schritte</span><span class="sxs-lookup"><span data-stu-id="05976-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="05976-103">Basierend auf Ihrer Problembeschreibung haben wir eine Lösung für Sie gefunden.</span><span class="sxs-lookup"><span data-stu-id="05976-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="05976-104">Die meisten Kunden konnten Ihr Problem selbst lösen, nachdem Sie unsere Dokumentation befolgen.</span><span class="sxs-lookup"><span data-stu-id="05976-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="05976-105">**Bearbeiten des Abonnement Administrators oder des Co-Administrators**</span><span class="sxs-lookup"><span data-stu-id="05976-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="05976-106">Der Konto Administrator kann beide Rollen bearbeiten, während der Abonnement Administrator nur Co-Administratoren im Azure- [Portal](https://ms.portal.azure.com/#home)ändern kann.</span><span class="sxs-lookup"><span data-stu-id="05976-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="05976-107">Hinzufügen oder Ändern von Administratoren für Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="05976-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="05976-108">**Aktualisieren des Abonnement Administrators oder des Co-Administrator für interne (Airs)-Abonnements**</span><span class="sxs-lookup"><span data-stu-id="05976-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="05976-109">Der Dienstadministrator oder der Co-Administrator kann diese Aktion mit den folgenden Schritten selbst ausführen:</span><span class="sxs-lookup"><span data-stu-id="05976-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="05976-110">Melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) an, und klicken Sie im linken Blatt auf **Kostenverwaltung + Abrechnung** .</span><span class="sxs-lookup"><span data-stu-id="05976-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="05976-111">Klicken Sie auf das positionselement mit Ihrem Abonnement.</span><span class="sxs-lookup"><span data-stu-id="05976-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="05976-112">Dadurch wird die Übersicht für Ihr Abonnement geöffnet.</span><span class="sxs-lookup"><span data-stu-id="05976-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="05976-113">Klicken Sie auf dem **Abonnement** -Blade auf **Eigenschaften**.</span><span class="sxs-lookup"><span data-stu-id="05976-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="05976-114">Klicken Sie auf die Schaltfläche **Dienstadministrator** .</span><span class="sxs-lookup"><span data-stu-id="05976-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="05976-115">Geben Sie die e-Mail-Adresse des Benutzers ein, den Sie als Dienst Administrator festlegen möchten, und klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="05976-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="05976-116">**Hinzufügen/Ändern/Entfernen eines Co-Administrators**</span><span class="sxs-lookup"><span data-stu-id="05976-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="05976-117">Melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) als Dienst Administrator an.</span><span class="sxs-lookup"><span data-stu-id="05976-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="05976-118">Öffnen Sie [Abonnements](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , und wählen Sie ein Abonnement aus.</span><span class="sxs-lookup"><span data-stu-id="05976-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="05976-119">(Co-Administratoren kann nur im Abonnement Bereich zugewiesen werden.)</span><span class="sxs-lookup"><span data-stu-id="05976-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="05976-120">Navigieren Sie zu **Access Control (IAM)**  >  **Classic Administrators** hinzufügen Sie  >    >  **Add Co-Administrator** , um den Bereich **Co-Admin hinzufügen** zu öffnen (wenn die Option Co-Administrator hinzufügen deaktiviert ist, bedeutet dies, dass Sie nicht über Berechtigungen verfügen).</span><span class="sxs-lookup"><span data-stu-id="05976-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="05976-121">Wählen Sie den Benutzer aus, den Sie hinzufügen möchten, und klicken Sie auf **Hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="05976-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="05976-122">**Weitere Informationen:**</span><span class="sxs-lookup"><span data-stu-id="05976-122">**Learn more:**</span></span>
- [<span data-ttu-id="05976-123">Hinzufügen eines Co-Administrators</span><span class="sxs-lookup"><span data-stu-id="05976-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="05976-124">Entfernen eines Co-Administrators</span><span class="sxs-lookup"><span data-stu-id="05976-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="05976-125">Ändern des Dienstadministrators</span><span class="sxs-lookup"><span data-stu-id="05976-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="05976-126">Anzeigen des Konto Administrators</span><span class="sxs-lookup"><span data-stu-id="05976-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="05976-127">Verwalten des Zugriffs über RBAC und Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="05976-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="05976-128">**Hinzufügen/Löschen von Benutzern mithilfe von Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="05976-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="05976-129">Sie können neue Benutzer hinzufügen oder vorhandene Benutzer aus ihrer Azure-Active Directory (Azure AD)-Organisation löschen:</span><span class="sxs-lookup"><span data-stu-id="05976-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="05976-130">Um einen neuen Benutzer hinzuzufügen, melden Sie sich als Benutzer Administrator für die Organisation im [Azure-Portal](https://ms.portal.azure.com/#home) an.</span><span class="sxs-lookup"><span data-stu-id="05976-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="05976-131">Wählen Sie **Azure Active Directory** aus, wählen Sie **Benutzer** aus, und klicken Sie dann auf **neuer Benutzer**.</span><span class="sxs-lookup"><span data-stu-id="05976-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="05976-132">Füllen Sie auf der Seite **Benutzer** die erforderlichen Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="05976-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="05976-133">Klicken Sie auf **Erstellen**.</span><span class="sxs-lookup"><span data-stu-id="05976-133">Click **Create**.</span></span> <span data-ttu-id="05976-134">Der Benutzer wird erstellt und dem Azure AD Mandanten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="05976-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="05976-135">**Weitere Informationen**:</span><span class="sxs-lookup"><span data-stu-id="05976-135">**Learn more**:</span></span>

- [<span data-ttu-id="05976-136">Hinzufügen eines neuen Benutzers</span><span class="sxs-lookup"><span data-stu-id="05976-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="05976-137">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="05976-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="05976-138">Hinzufügen oder Aktualisieren der Profilinformationen eines Benutzers mithilfe von Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="05976-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="05976-139">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="05976-139">**Recommended documents**</span></span>

- [<span data-ttu-id="05976-140">Was ist die rollenbasierte Zugriffssteuerung (Role-Based Access Control, RBAC)?</span><span class="sxs-lookup"><span data-stu-id="05976-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="05976-141">Grundlegendes zu den verschiedenen Rollen in Azure</span><span class="sxs-lookup"><span data-stu-id="05976-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="05976-142">Administratorrollenberechtigungen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="05976-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="05976-143">Lernprogramm: Gewähren des Zugriffs für einen Benutzer, der RBAC und das Azure-Portal verwendet</span><span class="sxs-lookup"><span data-stu-id="05976-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="05976-144">Problembehandlung bei RBAC in Azure</span><span class="sxs-lookup"><span data-stu-id="05976-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="05976-145">Organisieren Ihrer Ressourcen mit Azure-Verwaltungsgruppen</span><span class="sxs-lookup"><span data-stu-id="05976-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="05976-146">Anfordern einer Kopie von Azure Invoice per e-Mail</span><span class="sxs-lookup"><span data-stu-id="05976-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="05976-147">Vorgehensweise hinzufügen, aktualisieren oder Entfernen einer Kreditkarte oder Debitkarte aus Azure</span><span class="sxs-lookup"><span data-stu-id="05976-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="05976-148">Abonnement verwalten (reactivate/Cancel/Switch)</span><span class="sxs-lookup"><span data-stu-id="05976-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



