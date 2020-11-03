---
title: Übertragen des Besitzes von Azure-Abrechnungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840607"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="b171a-102">Übertragen des Besitzes von Azure-Abrechnungen</span><span class="sxs-lookup"><span data-stu-id="b171a-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="b171a-103">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) als Administrator des Abrechnungskontos mit dem Abonnement an, das Sie übertragen möchten.</span><span class="sxs-lookup"><span data-stu-id="b171a-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="b171a-104">Wenn Sie nicht genau wissen, ob Sie Administrator sind, oder wenn Sie ermitteln möchten, wer dies ist, lesen Sie [Ermitteln des Administrators des Abrechnungskontos](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="b171a-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="b171a-105">Suchen Sie nach **Kostenverwaltung und Abrechnung**.</span><span class="sxs-lookup"><span data-stu-id="b171a-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="b171a-106">Wählen Sie im linken Bereich **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="b171a-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="b171a-107">Je nach Zugriff müssen Sie möglicherweise einen Abrechnungsumfang und dann **Abonnements** oder **Azure-Abonnements** auswählen.</span><span class="sxs-lookup"><span data-stu-id="b171a-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="b171a-108">Wählen Sie **Übertragen des Besitzes von Abrechnungen** für das Abonnement, das Sie übertragen möchten.</span><span class="sxs-lookup"><span data-stu-id="b171a-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="b171a-109">Geben Sie die E-Mail-Adresse eines Benutzers ein, der ein Rechnungsadministrator des Kontos ist, das der neue Eigentümer für das Abonnement sein wird, und wählen Sie dann **Übertragungsanforderung** senden </span><span class="sxs-lookup"><span data-stu-id="b171a-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="b171a-110">Der Benutzer erhält eine E-Mail mit Anweisungen zur Überprüfung Ihrer Übertragungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="b171a-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="b171a-111">Um die Übertragungsanforderung zu genehmigen, wählt der Benutzer den Link in der E-Mail aus und folgt den Anweisungen.</span><span class="sxs-lookup"><span data-stu-id="b171a-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="b171a-112">**Hinweis** : Wenn Sie den Besitz von Abrechnungen Ihres Abonnements auf das Konto eines Benutzers in einem anderen Azure AD-Mandanten übertragen, werden alle [rollenbasierten Zugriffssteuerungen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) zur Verwaltung der Ressourcen im Abonnement dauerhaft entfernt.</span><span class="sxs-lookup"><span data-stu-id="b171a-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="b171a-113">Nur der neue Eigentümer hat Zugang zur Verwaltung der Ressourcen im Abonnement.</span><span class="sxs-lookup"><span data-stu-id="b171a-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="b171a-114">Weitere Informationen finden Sie unter [Übertragung des Abonnements an einen Benutzer in einem anderen Azure AD-Mandanten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b171a-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="b171a-115">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="b171a-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="b171a-116">Übertragen des Besitzes von Abrechnungen eines Azure-Abonnements auf ein anderes Konto</span><span class="sxs-lookup"><span data-stu-id="b171a-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="b171a-117">Informationen zum Übertragen des Besitzes von Abrechnungen für ein Azure-Abonnement</span><span class="sxs-lookup"><span data-stu-id="b171a-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="b171a-118">Übertragen von Abonnements für Visual Studio, Microsoft Partner Network (MPN) und Pay as you go Dev/Test</span><span class="sxs-lookup"><span data-stu-id="b171a-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="b171a-119">Übertragung des Besitzes – FAQ</span><span class="sxs-lookup"><span data-stu-id="b171a-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="b171a-120">Problembehandlung bei der Übertragung des Besitzes</span><span class="sxs-lookup"><span data-stu-id="b171a-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
