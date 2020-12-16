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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services – verschiebt alle RDFE-Dienste in ein anderes Abonnement.

**Ressourcen Verlagerung**

Azure-Ressourcen können mithilfe von Azure-Portal, Azure PowerShell, Azure CLI oder der Rest-API in ein anderes Azure-Abonnement oder eine Ressourcengruppe mit dem gleichen Abonnement verschoben werden, um Ressourcen zu verschieben.

Informationen zum Migrieren von Ressourcen finden Sie unter:

- [Prüfliste vor dem Verschieben von Ressourcen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Dienste, die verschoben werden können](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Vorgehensweise zum Überprüfen des verschiebe](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Verschiebe Anleitungen für Dienste](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Wenn Sie vorhandene Ressourcen in eine andere Ressourcengruppe oder ein anderes Abonnement migrieren möchten, können Sie Folgendes verwenden:

- [Azure-Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure-CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Lernprogramm: [Azure-Ressourcen in eine andere Ressourcengruppe oder ein anderes Abonnement migrieren](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Behandeln von Fehlern mit Azure Resource Manager**

In den folgenden Artikeln erfahren Sie mehr über einige häufige Azure-Bereitstellungsfehler und erhalten Informationen, um Sie zu beheben. Wenn Sie den Fehlercode für den Bereitstellungsfehler nicht finden können, finden Sie weitere Informationen untersuchen des Fehler [Codes](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Problembehandlung bei Bereitstellungsfehlern](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Problembehandlung beim Verschieben von Azure-Ressourcen in eine neue Ressourcengruppe oder ein Abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Beachten Sie, dass Sie Ihr Abonnement konvertieren müssen, wenn Sie ein Upgrade Ihres Azure-Abonnements durchführen möchten, beispielsweise von Free auf Pay-How-go wechseln.

- Informationen zum Upgrade einer kostenlosen Testversion finden Sie unter [Upgrade Ihrer kostenlosen Testversion oder Microsoft Imagine Azure-Abonnement für Pay-as-you-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Informationen zum Ändern eines Pay-as-you-go-Kontos finden Sie unter [Ändern Ihres Azure Pay-as-you-go-Abonnements für ein anderes Angebot](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Zum Hinzufügen oder Zuordnen eines Azure-Abonnements zu Ihrem Azure-Active Directory-Mandanten:**

1. Melden Sie sich an, und wählen Sie auf der [Seite Abonnements im Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)das Abonnement aus, das Sie verwenden möchten.
2. Wählen Sie **Change Directory** aus.
3. Überprüfen Sie alle angezeigten Warnungen, und wählen Sie dann **ändern** aus.
4. Das Verzeichnis wird für das Abonnement geändert, und Sie erhalten eine Erfolgsmeldung.
5. Verwenden Sie die *Verzeichnis* Umschalter, um zu Ihrem neuen Verzeichnis zu wechseln. Es kann bis zu 10 Minuten dauern, bis alles ordnungsgemäß angezeigt wird.

**Empfohlene Dokumente**

- [Übertragen des Besitzes eines Azure-Abonnements](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Ressourcen in neue Ressourcengruppe oder Abonnement migrieren](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Verwalten von Ressourcen mithilfe des Azure-Portals](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
