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
# <a name="transfer-azure-billing-ownership"></a>Übertragen des Besitzes von Azure-Abrechnungen

Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) als Administrator des Abrechnungskontos mit dem Abonnement an, das Sie übertragen möchten. Wenn Sie nicht genau wissen, ob Sie Administrator sind, oder wenn Sie ermitteln möchten, wer dies ist, lesen Sie [Ermitteln des Administrators des Abrechnungskontos](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Suchen Sie nach **Kostenverwaltung und Abrechnung**.
- Wählen Sie im linken Bereich **Abonnements** aus. Je nach Zugriff müssen Sie möglicherweise einen Abrechnungsumfang und dann **Abonnements** oder **Azure-Abonnements** auswählen.
- Wählen Sie **Übertragen des Besitzes von Abrechnungen** für das Abonnement, das Sie übertragen möchten.
- Geben Sie die E-Mail-Adresse eines Benutzers ein, der ein Rechnungsadministrator des Kontos ist, das der neue Eigentümer für das Abonnement sein wird, und wählen Sie dann **Übertragungsanforderung** senden 
- Der Benutzer erhält eine E-Mail mit Anweisungen zur Überprüfung Ihrer Übertragungsanforderung. Um die Übertragungsanforderung zu genehmigen, wählt der Benutzer den Link in der E-Mail aus und folgt den Anweisungen.

**Hinweis** : Wenn Sie den Besitz von Abrechnungen Ihres Abonnements auf das Konto eines Benutzers in einem anderen Azure AD-Mandanten übertragen, werden alle [rollenbasierten Zugriffssteuerungen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) zur Verwaltung der Ressourcen im Abonnement dauerhaft entfernt. Nur der neue Eigentümer hat Zugang zur Verwaltung der Ressourcen im Abonnement. Weitere Informationen finden Sie unter [Übertragung des Abonnements an einen Benutzer in einem anderen Azure AD-Mandanten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Empfohlene Dokumente**

- [Übertragen des Besitzes von Abrechnungen eines Azure-Abonnements auf ein anderes Konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informationen zum Übertragen des Besitzes von Abrechnungen für ein Azure-Abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Übertragen von Abonnements für Visual Studio, Microsoft Partner Network (MPN) und Pay as you go Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Übertragung des Besitzes – FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problembehandlung bei der Übertragung des Besitzes](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
