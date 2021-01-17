---
title: Zuweisen von Gruppen zu Azure AD-Rollen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875404"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="39e65-102">Zuweisen von Gruppen zu Azure AD-Rollen</span><span class="sxs-lookup"><span data-stu-id="39e65-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="39e65-103">Um eine Azure AD-Gruppe mit Autoritätsquelle in Azure AD zu einer Azure AD-Rolle zuzuweisen, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="39e65-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="39e65-104">Erstellen Sie eine neue Gruppe – Um eine neue Gruppe zu erstellen:</span><span class="sxs-lookup"><span data-stu-id="39e65-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="39e65-105">a.</span><span class="sxs-lookup"><span data-stu-id="39e65-105">a.</span></span> <span data-ttu-id="39e65-106">Melden Sie sich im Azure AD-Admin Center mit Berechtigungen für einen **Administrator für privilegierte Rollen** oder für einen **globalen Administrator** an.</span><span class="sxs-lookup"><span data-stu-id="39e65-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="39e65-107">b.</span><span class="sxs-lookup"><span data-stu-id="39e65-107">b.</span></span> <span data-ttu-id="39e65-108">Wählen Sie **Azure Active Directory > Gruppen > Alle Gruppen > Neue Gruppe** aus.</span><span class="sxs-lookup"><span data-stu-id="39e65-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="39e65-109">c.</span><span class="sxs-lookup"><span data-stu-id="39e65-109">c.</span></span> <span data-ttu-id="39e65-110">Erstellen Sie die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="39e65-110">Create the group.</span></span>

2. <span data-ttu-id="39e65-111">Weisen Sie der Gruppe die Rolle zu, entweder während der Erstellung der Gruppe oder nachdem die Gruppe erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="39e65-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="39e65-112">a.</span><span class="sxs-lookup"><span data-stu-id="39e65-112">a.</span></span> <span data-ttu-id="39e65-113">Um der Gruppe eine Rolle zum Zeitpunkt der Gruppenerstellung zuzuweisen, aktivieren Sie die Umschaltfläche **Azure AD-Rollen können der Gruppe zugewiesen werden** und erstellen Sie die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="39e65-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="39e65-114">b.</span><span class="sxs-lookup"><span data-stu-id="39e65-114">b.</span></span> <span data-ttu-id="39e65-115">Um der Gruppe eine Rolle zuzuweisen, nachdem sie erstellt wurde, navigieren Sie zur Registerkarte **Zugewiesene Rollen** für die neu erstellte Gruppe und weisen Sie der Gruppe die Rolle zu.</span><span class="sxs-lookup"><span data-stu-id="39e65-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="39e65-116">**Verwalten Sie die Mitgliedschaft in einer Gruppe, der eine Azure AD-Rolle** zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="39e65-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="39e65-117">Um eine standardmäßige Erhöhung von Rechten zu verhindern, können nur Administratoren für privilegierte Rollen und globale Administratoren die Mitgliedschaft einer Gruppe ändern, der eine Rolle zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="39e65-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="39e65-118">Sie können jedoch auswählen, ob Sie einen Besitzer für eine solche Gruppe auswählen möchten und diese Aufgabe delegieren.</span><span class="sxs-lookup"><span data-stu-id="39e65-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="39e65-119">Weitere Details darüber, wie Cloudgruppen zu Azure AD-Rollen zugewiesen werden, finden Sie unter [Zuweisen von AD-Rollen für Cloudgruppen](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="39e65-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="39e65-120">Weitere Details über Problembehandlung von Rollen, die Cloudgruppen zugewiesen werden, finden Sie unter [Problembehandlung von Rollen, die Cloudgruppen zugewiesen wurden](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="39e65-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





