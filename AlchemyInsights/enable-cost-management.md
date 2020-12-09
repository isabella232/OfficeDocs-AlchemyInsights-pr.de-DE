---
title: Aktivieren der Kostenverwaltung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599063"
---
# <a name="enable-cost-management"></a><span data-ttu-id="fdd3c-102">Aktivieren der Kostenverwaltung</span><span class="sxs-lookup"><span data-stu-id="fdd3c-102">Enable cost management</span></span>

<span data-ttu-id="fdd3c-103">**Was bedeutet "Kosten sind für Ihre Organisation deaktiviert?"?**</span><span class="sxs-lookup"><span data-stu-id="fdd3c-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="fdd3c-104">Organisationen, die Enterprise Agreement (EA) oder Microsoft-Kunden Vereinbarungs Konten (MCA) verwenden, können den Zugriff auf Kosteninformationen und Preisinformationen deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="fdd3c-105">Nachdem Sie sich beim Azure-Portal angemeldet haben, können Sie mit den Abrechnungs-APIs programmgesteuert Rechnungen (einmal eingecheckte) und Nutzungsdetails abrufen.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="fdd3c-106">**Vorgehensweise zulassen von weiteren Benutzern für den Zugriff auf Rechnungen**</span><span class="sxs-lookup"><span data-stu-id="fdd3c-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="fdd3c-107">Wechseln Sie zu **Abonnements Blatt** im Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="fdd3c-108">Wählen Sie **Rechnungen** aus, und klicken Sie dann **auf Rechnungen**.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="fdd3c-109">Aktivieren Sie den Zugriff, gefolgt von Speichern der Änderungen, damit Benutzer in Rollen mit Abonnementumfang Rechnungen herunterladen können.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="fdd3c-110">Der Konto Administrator kann auch konfigurieren, dass Rechnungen per e-Mail gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="fdd3c-111">Weitere Informationen finden Sie unter [Abrufen Ihrer Rechnung in e-Mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="fdd3c-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="fdd3c-112">**Vorgehensweise Hinzufügen von Benutzern zur Rolle "Abrechnungs Leser"**</span><span class="sxs-lookup"><span data-stu-id="fdd3c-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="fdd3c-113">Wechseln Sie zu **Abonnements Blatt** im Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="fdd3c-114">Wählen Sie **Zugriffssteuerung (IAM)** aus, und klicken Sie dann auf **Hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="fdd3c-115">Wählen Sie in der Seite **Rolle auswählen** die Option **Abrechnungs Leser** aus.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="fdd3c-116">Geben Sie die e-Mail-Adresse des Benutzers ein, den Sie einladen möchten, und klicken Sie dann auf **OK** , um die Einladung zu senden.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="fdd3c-117">Befolgen Sie die Anweisungen in der Einladungs-e-Mail zur Anmeldung als Abrechnungs Leser.</span><span class="sxs-lookup"><span data-stu-id="fdd3c-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="fdd3c-118">Weitere Informationen finden Sie unter [gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="fdd3c-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="fdd3c-119">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="fdd3c-119">**Recommended documents**</span></span>

- [<span data-ttu-id="fdd3c-120">Aktivieren von da und Ao-Ansichten über das EA-Portal</span><span class="sxs-lookup"><span data-stu-id="fdd3c-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="fdd3c-121">Kosten im Kosten Management</span><span class="sxs-lookup"><span data-stu-id="fdd3c-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="fdd3c-122">Unterstützte Microsoft Azure Angebote</span><span class="sxs-lookup"><span data-stu-id="fdd3c-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="fdd3c-123">Überprüfen der Kosten in der Kostenanalyse</span><span class="sxs-lookup"><span data-stu-id="fdd3c-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="fdd3c-124">Bereitstellen des Zugriffs auf Abrechnungsinformationen</span><span class="sxs-lookup"><span data-stu-id="fdd3c-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="fdd3c-125">Überprüfen des Zugriffs auf einen Microsoft-Kundenvertrag</span><span class="sxs-lookup"><span data-stu-id="fdd3c-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






