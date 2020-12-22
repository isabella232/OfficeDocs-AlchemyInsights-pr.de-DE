---
title: Wechsel zu Rechnungszahlung (Scheck/Überweisung)-Legacy WD
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
- "9004168"
- "7343"
ms.openlocfilehash: 1be90771f994e832960383b1cb5e0bee8f5b08f8
ms.sourcegitcommit: b561c339926fad609950ac92744c3cd91e0a68fa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/21/2020
ms.locfileid: "49722822"
---
# <a name="switch-to-invoice-pay-chequewire-transfer---legacy-wd"></a><span data-ttu-id="98853-102">Wechsel zu Rechnungszahlung (Scheck/Überweisung)-Legacy WD</span><span class="sxs-lookup"><span data-stu-id="98853-102">Switch to invoice pay (cheque/wire transfer) - Legacy WD</span></span>

<span data-ttu-id="98853-103">Wenn Sie zur Zahlung per Rechnung wechseln, bedeutet dies, dass Sie Ihre Rechnung innerhalb von 30 Tagen nach Rechnungsdatum bezahlen.</span><span class="sxs-lookup"><span data-stu-id="98853-103">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="98853-104">Um berechtigt zu sein, für Ihr Azure-Abonnement auf Rechnung zu bezahlen, senden Sie eine Anforderung an Azure Support.</span><span class="sxs-lookup"><span data-stu-id="98853-104">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="98853-105">Nachdem Ihre Anforderung genehmigt wurde, können Sie ein Abonnement für Rechnung in das Azure- [Portal](https://portal.azure.com/)auf Rechnungszahlung umschalten.</span><span class="sxs-lookup"><span data-stu-id="98853-105">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="98853-106">**Lesen Sie die folgenden Anforderungen/Einschränkungen für das Anfordern von Rechnungs Zahlungsoptionen, bevor Sie fortfahren:**</span><span class="sxs-lookup"><span data-stu-id="98853-106">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="98853-107">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an, und navigieren Sie zu Zahlungsmethoden.</span><span class="sxs-lookup"><span data-stu-id="98853-107">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="98853-108">Prüfen Sie, ob Sie bereits für die Rechnungszahlung vorab genehmigt wurden.</span><span class="sxs-lookup"><span data-stu-id="98853-108">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="98853-109">Der Rechnungs Lohn steht nur für Geschäftskonten zur Verfügung, nicht für persönliche Konten.</span><span class="sxs-lookup"><span data-stu-id="98853-109">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="98853-110">Sie müssen alle ausstehenden Gebühren bezahlen, bevor Sie zum Rechnungs Gehalt wechseln.</span><span class="sxs-lookup"><span data-stu-id="98853-110">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="98853-111">Das Support Team prüft das Konto, um festzustellen, ob es für den Rechnungs Zahlungsmodus berechtigt ist.</span><span class="sxs-lookup"><span data-stu-id="98853-111">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="98853-112">Der Rechnungs Zahlungsmodus wird für Drittanbieterdienste von Marketplace nicht unterstützt; Wenn Sie beabsichtigen, ein aktuelles Abonnement auf eine Rechnung umzuschalten, die Marketplace-oder 3rd Party-Dienste enthält, müssen diese Dienste vor dem Wechsel gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="98853-112">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="98853-113">Kaufen Sie für zukünftige Marketplace-Dienste zunächst ein separates Abonnement auf Kreditkarte, und kaufen oder stellen Sie dann Marketplace-Drittanbieterdienste ein.</span><span class="sxs-lookup"><span data-stu-id="98853-113">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="98853-114">Wenn Sie auf Rechnung bezahlen umstellen, können Sie nicht wieder auf Kredit-oder Debitkarten-Zahlung zurückwechseln.</span><span class="sxs-lookup"><span data-stu-id="98853-114">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="98853-115">*Sobald Sie zur Zahlung per Rechnung genehmigt* haben, können Sie Ihr Azure-Abonnement auf den Rechnung per Scheck oder Überweisung im Azure- [Portal](https://portal.azure.com/)umschalten.</span><span class="sxs-lookup"><span data-stu-id="98853-115">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="98853-116">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="98853-116">To do that:</span></span>

1. <span data-ttu-id="98853-117">Melden Sie sich [](https://portal.azure.com/)   als Konto Administrator beim Azure-Portal an.</span><span class="sxs-lookup"><span data-stu-id="98853-117">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="98853-118">Suchen und wählen Sie **Kosten Management + Abrechnung**.</span><span class="sxs-lookup"><span data-stu-id="98853-118">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="98853-119">Wählen Sie das Abonnement aus, das Sie zur Rechnungszahlung umschalten möchten.</span><span class="sxs-lookup"><span data-stu-id="98853-119">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="98853-120">Wählen Sie **Zahlungsmethoden** aus.</span><span class="sxs-lookup"><span data-stu-id="98853-120">Select **Payment methods**.</span></span>
3. <span data-ttu-id="98853-121">Klicken Sie in der Befehlsleiste auf die Schaltfläche **Zahlung per Rechnung** .</span><span class="sxs-lookup"><span data-stu-id="98853-121">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="98853-122">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="98853-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="98853-123">Anfordern/herunterladen/anzeigen ihrer Azure-Abrechnungs Rechnung und Nutzungsdaten</span><span class="sxs-lookup"><span data-stu-id="98853-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="98853-124">So senden Sie Azure-Rechnungen direkt an Ihren Posteingang</span><span class="sxs-lookup"><span data-stu-id="98853-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="98853-125">Bezahlung per Rechnung</span><span class="sxs-lookup"><span data-stu-id="98853-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="98853-126">Grundlegendes zu detaillierten Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="98853-126">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="98853-127">Verstehen von Ausdrücken auf Ihrer Rechnung</span><span class="sxs-lookup"><span data-stu-id="98853-127">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="98853-128">Übertragen des Besitzes</span><span class="sxs-lookup"><span data-stu-id="98853-128">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
