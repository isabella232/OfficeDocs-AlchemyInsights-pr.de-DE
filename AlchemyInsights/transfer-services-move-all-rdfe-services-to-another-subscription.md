---
title: Transfer Services – verschiebt alle RDFE-Dienste in ein anderes Abonnement.
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681476"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="2b240-102">Transfer Services – verschiebt alle RDFE-Dienste in ein anderes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="2b240-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="2b240-103">**Ressourcen Verlagerung**</span><span class="sxs-lookup"><span data-stu-id="2b240-103">**Move resources**</span></span>

<span data-ttu-id="2b240-104">Azure-Ressourcen können mithilfe von Azure-Portal, Azure PowerShell, Azure CLI oder der Rest-API in ein anderes Azure-Abonnement oder eine Ressourcengruppe mit dem gleichen Abonnement verschoben werden, um Ressourcen zu verschieben.</span><span class="sxs-lookup"><span data-stu-id="2b240-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="2b240-105">Informationen zum Migrieren von Ressourcen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="2b240-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="2b240-106">Prüfliste vor dem Verschieben von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="2b240-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="2b240-107">Dienste, die verschoben werden können</span><span class="sxs-lookup"><span data-stu-id="2b240-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="2b240-108">Vorgehensweise zum Überprüfen des verschiebe</span><span class="sxs-lookup"><span data-stu-id="2b240-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="2b240-109">Verschiebe Anleitungen für Dienste</span><span class="sxs-lookup"><span data-stu-id="2b240-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="2b240-110">Wenn Sie vorhandene Ressourcen in eine andere Ressourcengruppe oder ein anderes Abonnement migrieren möchten, können Sie Folgendes verwenden:</span><span class="sxs-lookup"><span data-stu-id="2b240-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="2b240-111">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="2b240-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="2b240-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2b240-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="2b240-113">Azure-CLI</span><span class="sxs-lookup"><span data-stu-id="2b240-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="2b240-114">REST API</span><span class="sxs-lookup"><span data-stu-id="2b240-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="2b240-115">Lernprogramm: [Azure-Ressourcen in eine andere Ressourcengruppe oder ein anderes Abonnement migrieren](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="2b240-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="2b240-116">**Behandeln von Fehlern mit Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="2b240-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="2b240-117">In den folgenden Artikeln erfahren Sie mehr über einige häufige Azure-Bereitstellungsfehler und erhalten Informationen, um Sie zu beheben.</span><span class="sxs-lookup"><span data-stu-id="2b240-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="2b240-118">Wenn Sie den Fehlercode für den Bereitstellungsfehler nicht finden können, finden Sie weitere Informationen untersuchen des Fehler [Codes](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="2b240-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="2b240-119">Problembehandlung bei Bereitstellungsfehlern</span><span class="sxs-lookup"><span data-stu-id="2b240-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="2b240-120">Problembehandlung beim Verschieben von Azure-Ressourcen in eine neue Ressourcengruppe oder ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="2b240-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="2b240-121">Beachten Sie, dass Sie Ihr Abonnement konvertieren müssen, wenn Sie ein Upgrade Ihres Azure-Abonnements durchführen möchten, beispielsweise von Free auf Pay-How-go wechseln.</span><span class="sxs-lookup"><span data-stu-id="2b240-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="2b240-122">Informationen zum Upgrade einer kostenlosen Testversion finden Sie unter [Upgrade Ihrer kostenlosen Testversion oder Microsoft Imagine Azure-Abonnement für Pay-as-you-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="2b240-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="2b240-123">Informationen zum Ändern eines Pay-as-you-go-Kontos finden Sie unter [Ändern Ihres Azure Pay-as-you-go-Abonnements für ein anderes Angebot](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="2b240-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="2b240-124">**Zum Hinzufügen oder Zuordnen eines Azure-Abonnements zu Ihrem Azure-Active Directory-Mandanten:**</span><span class="sxs-lookup"><span data-stu-id="2b240-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="2b240-125">Melden Sie sich an, und wählen Sie auf der [Seite Abonnements im Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)das Abonnement aus, das Sie verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="2b240-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="2b240-126">Wählen Sie **Change Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="2b240-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="2b240-127">Überprüfen Sie alle angezeigten Warnungen, und wählen Sie dann **ändern** aus.</span><span class="sxs-lookup"><span data-stu-id="2b240-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="2b240-128">Das Verzeichnis wird für das Abonnement geändert, und Sie erhalten eine Erfolgsmeldung.</span><span class="sxs-lookup"><span data-stu-id="2b240-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="2b240-129">Verwenden Sie die *Verzeichnis* Umschalter, um zu Ihrem neuen Verzeichnis zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="2b240-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="2b240-130">Es kann bis zu 10 Minuten dauern, bis alles ordnungsgemäß angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="2b240-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="2b240-131">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="2b240-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="2b240-132">Übertragen des Besitzes eines Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="2b240-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="2b240-133">Ressourcen in neue Ressourcengruppe oder Abonnement migrieren</span><span class="sxs-lookup"><span data-stu-id="2b240-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="2b240-134">Verwalten von Ressourcen mithilfe des Azure-Portals</span><span class="sxs-lookup"><span data-stu-id="2b240-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
