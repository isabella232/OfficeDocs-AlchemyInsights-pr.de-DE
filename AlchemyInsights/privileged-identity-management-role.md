---
title: Rolle "privilegierte Identitätsverwaltung"
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086376"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="3c2d9-102">Rolle "PIM (Privileged Identity Management)"</span><span class="sxs-lookup"><span data-stu-id="3c2d9-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="3c2d9-103">**Berechtigungen werden nach dem Aktivieren einer Rolle nicht erteilt.**</span><span class="sxs-lookup"><span data-stu-id="3c2d9-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="3c2d9-104">Wenn Sie eine Rolle in Azure AD privilegierten Identitätsverwaltung (PIM) aktivieren, wird die Aktivierung möglicherweise nicht sofort an alle Portale weitergegeben, die die privilegierte Rolle benötigen.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="3c2d9-105">In einigen Fällen kann es vorkommen, dass die Änderung nicht sofort wirksam wird, auch wenn die Änderung weitergegeben wird.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="3c2d9-106">Wenn Ihre Aktivierung verzögert wird, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="3c2d9-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="3c2d9-107">Melden Sie sich im Azure-Portal ab, und melden Sie sich dann wieder an.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="3c2d9-108">Wenn Sie eine Azure AD Rolle oder eine Azure-Ressourcenrolle aktivieren, werden die Phasen der Aktivierung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="3c2d9-109">Sobald alle Phasen abgeschlossen sind, wird der Link "Abmelden" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="3c2d9-110">Sie können diesen Link verwenden, um sich abzumelden. Dadurch werden die meisten Fälle für die Aktivierungsverzögerung gelöst.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="3c2d9-111">Stellen Sie in PIM sicher, dass Sie als Mitglied der Rolle aufgeführt sind.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="3c2d9-112">Wenn Sie die Rolle Exchange-Administrator aktivieren, stellen Sie sicher, dass Sie sich abmelden und wieder anmelden.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="3c2d9-113">Wenn das Problem weiter besteht, öffnen Sie ein Support Ticket, und stellen Sie dieses als Problem herauf.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="3c2d9-114">Wenn Sie Ihre Exchange-Administrator Rolle für den Zugriff auf das Security and Compliance Center verwenden, lesen Sie den nächsten Schritt.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="3c2d9-115">Wenn Sie eine Rolle für den Zugriff auf das Security and Compliance Center aktivieren oder die SharePoint-Administrator Rolle aktivieren, tritt eine Aktivierungsverzögerung von ein paar Minuten bis zu einigen Stunden ein.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="3c2d9-116">Dies ist ein bekanntes Problem, und wir arbeiten aktiv mit diesen Teams zusammen, um dieses Problem so schnell wie möglich zu beheben.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="3c2d9-117">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="3c2d9-117">For more information, see:</span></span>

- [<span data-ttu-id="3c2d9-118">Aktivieren von "meine Azure AD"-Rollen in PIM</span><span class="sxs-lookup"><span data-stu-id="3c2d9-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="3c2d9-119">Aktivieren von My Azure Resource Roles in PIM</span><span class="sxs-lookup"><span data-stu-id="3c2d9-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="3c2d9-120">**Berechtigungen werden nach dem Deaktivieren einer Rolle nicht entfernt, oder die Rollen Aktivierung läuft ab.**</span><span class="sxs-lookup"><span data-stu-id="3c2d9-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="3c2d9-121">Wenn Sie eine Rolle in Azure AD privilegierten Identitätsverwaltung oder beim Ablauf einer Rollen Aktivierungs Periode deaktivieren, kann es zu Verzögerungen kommen, in denen Sie weiterhin auf Zugriff haben.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="3c2d9-122">Wenn Ihre Deaktivierung verzögert wird, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="3c2d9-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="3c2d9-123">Wenn Sie die Exchange-Administrator Rolle deaktivieren oder der Aktivierungszeitraum für die Rolle abgelaufen ist und Sie eine erhebliche Verzögerung feststellen, bevor die Berechtigungen entfernt wurden, öffnen Sie ein Support Ticket, und teilen Sie Ihrem Supporttechniker mit, wie Sie ein Ticket mit dem Team für die privilegierte Zugriffsverwaltung ("PAM") in Office zu diesem Problem einreichen können.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="3c2d9-124">Wenn der Aktivierungszeitraum abgelaufen ist, Sie aber dennoch die Browsersitzung geöffnet haben, schließen Sie den Browser.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="3c2d9-125">Sie können die Rolle weiterhin verwenden, bis Sie diese Sitzung schließen.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="3c2d9-126">Dies ist ein bekanntes Problem, und wir suchen eine mögliche Lösung, um jede Sitzung aktiv aufzuheben, nachdem die Aktivierung abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="3c2d9-127">Wenn sich Ihre Verzögerung von diesen beiden Szenarien unterscheidet, öffnen Sie ein Support Ticket.</span><span class="sxs-lookup"><span data-stu-id="3c2d9-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
