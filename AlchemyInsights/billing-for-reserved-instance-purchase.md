---
title: Abrechnung des Kaufs reservierter Instanzen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816006"
---
# <a name="billing-for-reserved-instance-purchase"></a>Abrechnung des Kaufs reservierter Instanzen

Der Kauf reservierter Instanzen wird über die Zahlungsmethode abgerechnet, die mit dem Abonnement verknüpft ist, das Sie zum Kaufzeitpunkt auswählen. Bei dem Abonnement muss es sich um ein Enterprise Agreement (Angebotsnummer: MS-AZR-0017P), Pay-As-You-Go (Angebotsnummer: MS-AZR-0003P), eine Microsoft-Kundenvereinbarung oder CSP handeln.

- Bei einem Enterprise-Abonnement werden die Gebühren von dem Saldo der finanziellen Verpflichtung des Abonnements abgezogen, oder als Überschreitung berechnet.
- Bei einem Pay-As-You-Go-Abonnement werden die Gebühren über die Kreditkarte oder Zahlungsmethode des Abonnements abgerechnet.

**Reservierung stornieren**

- **Self-Service:** Sie können eine reservierte Instanz mithilfe von [Azure Portal-](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)selbst stornieren oder austauschen. Wählen Sie die Reservierung aus, und klicken Sie auf zurückerstatten oder austauschen. Bitte beachten Sie, dass Sie auf dem Reservierungsauftrag Inhaberzugriff haben müssen, um austauschen oder zurückerstatten zu können. Wenn Sie nur auf die Reservierung zugreifen, können Sie die Rückerstattung oder den Umtausch nicht fortsetzen. Bitten Sie den Besitzer des Reservierungsauftrags, Ihnen Inhaberzugriff auf den Reservierungsauftrag zu erteilen.
- **Exchange-Richtlinie:** Sie können eine Reservierung für eine andere Reservierung desselben Typs tauschen – es gibt **kein Bußgeld** bei Reservierungsaustausch. Die Gesamtverpflichtung mit neuer Buchung sollte höher sein als die Summe der Erstattungsbeträge der ausgetauschten Reservationen und der künftigen monatlichen Zahlungen (sofern zutreffend).
- **Erstattungsrichtlinie:** Summe der Erstattung und der annullierten künftigen Zahlungen dürfen in einem laufenden 12-monatigen Fenster $50.000 USD nicht überschreiten. Wir **berechnen aktuell kein Bußgeld** für Erstattungen, aber könnten sie für zukünftige Erstattungen berechnen.

**Ausnahmen:** Self-Service-Umtausch- und Stornierungsmöglichkeit sind für Kunden in US-Behörden nicht verfügbar

- **API / PS / CLI** Support steht nicht für Stornierung und Rückerstattungen zur Verfügung [Self-Service-Umtausche und Erstattungen für Azure-Reservierungen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Self-Service Exchange- und Stornierungsmöglichkeit sind für Kunden von US Government Enterprise Agreement nicht verfügbar. Weitere US Government-Abonnementtypen einschließlich Nutzungsbasierte Zahlung und CSP werden unterstützt

Weitere Informationen: [wie Rückgabe-und Exchange-Transaktionen verarbeitet werden](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Weitere Informationen: [Exchange-und Erstattungsrichtlinien](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) weitere Fragen: [besuchen Sie reservierte Instanz-Dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tauschen einer vorhandenen reservierten Instanz (Self-Service)**

Sie können eine Reservierung für eine andere Reservierung desselben Typs tauschen. Sie können auch eine Reservierung von bis zu $50.000 USD pro Jahr erstatten, wenn Sie sie nicht mehr benötigen. Self-Service Exchange- und Stornierungsmöglichkeit sind für Kunden von US Government Enterprise Agreement nicht verfügbar. Weitere US Government-Abonnementtypen einschließlich Nutzungsbasierte Zahlung und CSP werden unterstützt. Sie müssen auf dem Reservierungsauftrag Inhaberzugriff haben, um austauschen oder zurückerstatten zu können.

In den folgenden Schritten wird beschrieben, wie Sie die Transaktion ausführen.

1. Melden Sie sich bei Ihrem [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)an. Wählen Sie die Reservierungen aus, die Sie zurückerstatten möchten, und klicken Sie auf **Exchange** 2. Wählen Sie das VM-Produkt aus, das Sie kaufen möchten, und geben Sie eine Menge ein. Stellen Sie sicher, dass die neue Einkaufssumme mehr ist, als die Rückgabe Summe [vor dem Kauf die richtige Größe bestimmt](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. überprüfen und Abschließen der Transaktion

**Rückerstattung für eine reservierte Instanz**

Wenn Sie eine Reservierung zurückerstatten möchten, wechseln Sie zu **Reservierungsdetails** und klicken Sie auf **Rückerstattung**

**Anteilige Rückerstattung:**

**Pro-ration-und mindestanforderungs Beispiele für Rückerstattung und Exchange** Beispiel für die Vorabreservierung:

- Sie kaufen einen RI-Jahreszeitraum für $120 am 1. Januar.
- Am 7. April möchten Sie diese Reservierung zurückerstatten oder austauschen.
- Da die Reservierung seit 97 Tagen erfolgt, erhalten Sie (1-97/365) * $120 zurück. (d. h. $88,1). Derzeit gibt es kein Bußgeld für Erstattungen
- Bei einem Umtausch sollte Ihr neuer Kauf größer als $88,1 sein
- Es gibt kein Bußgeld für Rückerstattung zur Zeit

**Beispiel für einen Abrechnungsplan:**

- Sie kaufen einen RI-Jahreszeitraum für $10 pro Monat
- Am 7. April möchten Sie diese Reservierung zurückerstatten oder austauschen.
- Seit der letzten Zahlung 7 Tage, erhalten Sie (1-7/31) * $10 zurück. (d. h. $7,74).
- Die zukünftig stornierten Zahlungen sind $80. Derzeit gibt es kein Bußgeld für Erstattungen
- Bei dieser Kündigung wird $87,74 von Ihrem $50.000-Erstattungslimit abgezogen.
- Bei einem Umtausch sollte Ihr neuer Kauf größer als $87,74 sein

**Rechnung für den letzten Abrechnungszeitraum kann nicht angezeigt werden**

Einige mögliche Gründe, weshalb eine Rechnung möglicherweise nicht angezeigt wird:

- Sie haben einen monatlichen Kreditbetrag mit Ihrem Abonnement, den Sie nicht überschritten haben, oder Sie haben eine ﻿kostenlose Testversion. Eine Rechnung wird nur generiert, wenn Sie Geld Schulden.
- Es ist weniger als 30 Tage nach dem Tag, an dem Sie Azure abonniert haben.
- Die Rechnung wird noch nicht generiert. Warten bis zum Ende des Abrechnungszeitraums
- Wenn Sie nicht der Konto Administrator sind, stehen Ihnen ältere Rechnungen möglicherweise nicht zur Verfügung.

**Laden Sie Ihre Rechnung aus dem Azure-Portal herunter (. pdf)**

- Wählen Sie Ihr Abonnement auf der Seite " [Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) " im Azure-Portal als [Benutzer mit Zugriff auf Rechnungen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support) aus.
- **Rechnungen** auswählen
- Klicken Sie auf **Rechnung herunterladen** , um eine Kopie Ihrer PDF-Rechnung anzuzeigen. Wenn die Meldung **nicht verfügbar** ist, finden Sie weitere Informationen unter [Warum wird für den letzten Abrechnungszeitraum keine Rechnung angezeigt?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Ihre Rechnung per e-Mail erhalten (. pdf)**

- Wählen Sie Ihr Abonnement auf der Seite [Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) aus. Klicken Sie auf **Rechnungen** und dann auf meine Rechnung per e-Mail
- Klicken Sie auf **Anmelden** und akzeptieren Sie die Bedingungen. Sie müssen sich für jedes Abonnement anmelden, das Sie besitzen.

Hinweis: Wenn Sie keine e-Mails erhalten, nachdem Sie die folgenden Schritte ausgeführt haben, stellen Sie sicher, dass Ihre e-Mail-Adresse in den [Kommunikationseinstellungen in Ihrem Profil](https://account.windowsazure.com/profile) richtig ist.

**Herunterladen Ihrer Verwendungsdaten aus dem Azure-Portal**

- Melden Sie sich beim [Azure Account Center](https://account.windowsazure.com/Subscriptions) als [Konto Administrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) an.
- Wählen Sie das Abonnement aus, für das die Rechnungs-und Nutzungsinformationen verwendet werden sollen.
- **Abrechnungsverlauf** auswählen
- Wählen Sie **aktuelle Anweisung anzeigen** aus, um eine Schätzung ihrer Gebühren zu dem Zeitpunkt anzuzeigen, zu dem die Schätzung generiert wurde.
- Wählen Sie **Download Usage** aus, um die täglichen Nutzungsdaten als CSV-Datei herunterzuladen. Wenn zwei Versionen verfügbar sind, laden Sie Version 2 herunter.

Weitere Fragen: [reservierte Instanzdokumente besuchen](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Empfohlene Dokumentationen**

- [Abrechnungsgrundlagen](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Grundlegendes zur Anwendung des Rabatts für reservierte Instanzen](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Herunterladen oder Anzeigen Ihrer Azure-Abrechnungs Rechnung und der täglichen Nutzungsdaten](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Grundlegendes zur Anwendung des Rabatts für reservierte Instanzen](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Grundlegendes zur Verwendung von reservierten Instanzen für Ihr Pay-as-you-go-Abonnement](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Grundlegendes zur Verwendung reservierter Instanzen für Ihre Unternehmensregistrierung](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-Software Kosten, die nicht in reservierten Instanzen enthalten sind](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reservierte Instanzen im Partner Programm für den zentralen Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)