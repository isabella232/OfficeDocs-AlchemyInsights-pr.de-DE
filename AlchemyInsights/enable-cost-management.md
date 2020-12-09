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
# <a name="enable-cost-management"></a>Aktivieren der Kostenverwaltung

**Was bedeutet "Kosten sind für Ihre Organisation deaktiviert?"?**

Organisationen, die Enterprise Agreement (EA) oder Microsoft-Kunden Vereinbarungs Konten (MCA) verwenden, können den Zugriff auf Kosteninformationen und Preisinformationen deaktivieren.

Nachdem Sie sich beim Azure-Portal angemeldet haben, können Sie mit den Abrechnungs-APIs programmgesteuert Rechnungen (einmal eingecheckte) und Nutzungsdetails abrufen.

**Vorgehensweise zulassen von weiteren Benutzern für den Zugriff auf Rechnungen**

1. Wechseln Sie zu **Abonnements Blatt** im Azure-Portal.
2. Wählen Sie **Rechnungen** aus, und klicken Sie dann **auf Rechnungen**.
3. Aktivieren Sie den Zugriff, gefolgt von Speichern der Änderungen, damit Benutzer in Rollen mit Abonnementumfang Rechnungen herunterladen können.

> [!NOTE]
> Der Konto Administrator kann auch konfigurieren, dass Rechnungen per e-Mail gesendet werden. Weitere Informationen finden Sie unter [Abrufen Ihrer Rechnung in e-Mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Vorgehensweise Hinzufügen von Benutzern zur Rolle "Abrechnungs Leser"**

1. Wechseln Sie zu **Abonnements Blatt** im Azure-Portal.
2. Wählen Sie **Zugriffssteuerung (IAM)** aus, und klicken Sie dann auf **Hinzufügen**.
3. Wählen Sie in der Seite **Rolle auswählen** die Option **Abrechnungs Leser** aus.
4. Geben Sie die e-Mail-Adresse des Benutzers ein, den Sie einladen möchten, und klicken Sie dann auf **OK** , um die Einladung zu senden.
5. Befolgen Sie die Anweisungen in der Einladungs-e-Mail zur Anmeldung als Abrechnungs Leser. Weitere Informationen finden Sie unter [gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Empfohlene Dokumente**

- [Aktivieren von da und Ao-Ansichten über das EA-Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kosten im Kosten Management](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Unterstützte Microsoft Azure Angebote](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Überprüfen der Kosten in der Kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Bereitstellen des Zugriffs auf Abrechnungsinformationen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Überprüfen des Zugriffs auf einen Microsoft-Kundenvertrag](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






