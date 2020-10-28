---
title: Abonnement Zugriff
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773774"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="c4403-102">Das Anmelden in Azure kann aufgrund von Browserproblemen nicht möglich sein (Browser hängt, dreht sich weiter, wird nicht herunterladen usw.)</span><span class="sxs-lookup"><span data-stu-id="c4403-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="c4403-103">Möglicherweise sind Sie von einem Ausfall betroffen.</span><span class="sxs-lookup"><span data-stu-id="c4403-103">You might be impacted by an outage.</span></span> <span data-ttu-id="c4403-104">Überprüfen Sie, ob ein ständiger Ausfall vorliegt: [Azure-Integritäts Status](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="c4403-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="c4403-105">Melden Sie sich bei allen aktiven Azure-Sitzungen ab.</span><span class="sxs-lookup"><span data-stu-id="c4403-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="c4403-106">Starten Sie einen in-private-oder Inkognito-Modus Ihres Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="c4403-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="c4403-107">Sie können auch versuchen, Browser zu aktualisieren, einen anderen Browser zu verwenden, Cache-Cookies zu löschen, wenn oben nicht funktioniert.</span><span class="sxs-lookup"><span data-stu-id="c4403-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="c4403-108">Weitere Informationen: [Problembehandlung bei Anmeldeproblemen](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="c4403-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="c4403-109">**Zugriff auf Abonnements nicht möglich**</span><span class="sxs-lookup"><span data-stu-id="c4403-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="c4403-110">Stellen Sie im [Azure-Portal](https://portal.azure.com/)sicher, dass das richtige Azure-Verzeichnis aus dem Konto oben rechts ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="c4403-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="c4403-111">Stellen Sie im [Azure-Konto Center](https://account.windowsazure.com/Subscriptions)sicher, dass das verwendete Konto der Konto Administrator ist.</span><span class="sxs-lookup"><span data-stu-id="c4403-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="c4403-112">Weitere Informationen: [Problembehandlung bei nicht gefundenen Abonnements](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c4403-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="c4403-113">**Zugriff auf Abrechnungsverlauf nicht möglich**</span><span class="sxs-lookup"><span data-stu-id="c4403-113">**Unable to access billing history**</span></span>

<span data-ttu-id="c4403-114">Der Konto Administrator muss sicherstellen, dass der Benutzer, der auf die Abrechnungsinformationen zugreift, im Azure Active Directory als Gastbenutzer hinzugefügt wird: [einen neuen Benutzer hinzufügen oder löschen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c4403-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c4403-115">Dem Benutzer muss dann eine globale Administratorrolle zugewiesen werden: [Zuweisen von Rollen zu Benutzern](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c4403-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c4403-116">Veröffentlichen Sie dies, kann dem Benutzer mithilfe von RBAC-Richtlinien ein Abrechnungs Zugriff gewährt werden: [gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c4403-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c4403-117">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="c4403-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="c4403-118">Ich kann mich nicht zum Verwalten des Azure-Abonnements anmelden.</span><span class="sxs-lookup"><span data-stu-id="c4403-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)