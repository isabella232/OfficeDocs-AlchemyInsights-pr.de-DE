---
title: Abrechnung für den Kauf einer reservierten Instanz
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820321"
---
# <a name="billing-for-reserved-instance-purchase"></a>Abrechnung für den Kauf einer reservierten Instanz

Der reservierte Instanzkauf wird der Zahlungsmethode in Rechnung gestellt, die an das Abonnement gebunden ist, das Sie zum Zeitpunkt des Kaufs auswählen. Der Abonnementtyp muss ein Unternehmensvertrag (Angebotsnummer: MS-AZR-0017P), Pay-As-You-Go (Angebotsnummer: MS-AZR-0003P), Microsoft Customer Agreement oder CSP sein.

- Für ein Unternehmensabonnement werden die Gebühren vom geldpolitischen Verpflichtungssaldo der Registrierung abgezogen oder als Übergewicht in Rechnung gestellt.
- Für Das Pay-As-You-Go-Abonnement werden die Gebühren der Kreditkarte oder der Zahlungsmethode für Rechnungen für das Abonnement in Rechnung gestellt.

**Reservierung abbrechen**

- **Self-Service:** Sie können eine reservierte Instanz selbst über das [Azure-Portal abbrechen oder austauschen.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Wählen Sie die Reservierung aus, und klicken Sie auf Rückerstattung oder Umtausch. Beachten Sie, dass Sie über Besitzerzugriff auf die Reservierungsbestellung zum Umtausch oder zur Rückerstattung verfügen müssen. Durch den Zugriff auf die Reservierung können Sie nicht mit der Rückerstattung oder dem Austausch fortfahren. Bitten Sie den Besitzer der Reservierungsbestellung, Ihnen Zugriff auf die Reservierungsbestellung zu geben.
- **Exchange-Richtlinie:** Sie können eine Reservierung gegen eine andere Reservierung desselben Typs austauschen – es gibt keine Strafen für den **Reservierungswechsel.** Die Gesamtverpflichtung bei neuer Reservierung sollte größer sein als die Summe des Erstattungsbetrags der getauschten Reservierung und die zukünftigen monatlichen Zahlungen (sofern zutreffend)
- **Erstattungsrichtlinie:** Die Summe der Rückerstattung und der stornierten zukünftigen Zahlungen darf 50.000 USD in einem 12-Monat-Rollfenster nicht überschreiten. Wir berechnen **derzeit keine Strafen für** Rückerstattungen, könnten sie aber für zukünftige Rückerstattungen berechnen.

**Ausnahmen:** Die Self-Service-Exchange- und Cancel-Funktion ist für Us Government Konzernvertrag verfügbar

- **API/PS/CLI-Support** steht für Stornierungen und Rückerstattungen nicht zur Verfügung [Self-Service-Austausch und Rückerstattungen für Azure-Reservierungen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Die Self-Service-Exchange- und Cancel-Funktion ist für Us Government Konzernvertrag verfügbar. Andere Us Government-Abonnementtypen, einschließlich Pay-As-You-Go und CSP, werden unterstützt.

Weitere Informationen : [Verarbeiten von Rückgabe- und Exchangetransaktionen](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Weitere Informationen : [Exchange- und Rückerstattungsrichtlinien](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Weitere Fragen: Besuchen Sie [reservierte Instanz-Dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange einer vorhandenen reservierten Instanz (Self-Service)**

Sie können eine Reservierung gegen eine andere Reservierung desselben Typs austauschen. Sie können eine Reservierung auch bis zu 50.000 USD pro Jahr zurückerstatten, wenn Sie sie nicht mehr benötigen. Die Self-Service-Exchange- und Cancel-Funktion ist für Us Government Konzernvertrag verfügbar. Andere Us Government-Abonnementtypen, einschließlich Pay-As-You-Go und CSP, werden unterstützt. Sie müssen über Besitzerzugriff auf die Reservierungsbestellung verfügen, um eine vorhandene Reservierung umtauschen oder zurückerstatten zu können.

In den folgenden Schritten wird das Verfahren zum Abschließen der Transaktion beschrieben.

1.Melden Sie sich bei Ihrem [Azure-Portal an.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Wählen Sie die Reservierungen aus, die Sie zurückerstatten möchten, und klicken Sie auf **Exchange** 2.Wählen Sie das vm-Produkt aus, das Sie kaufen möchten, und geben Sie eine Menge ein. Stellen Sie sicher, dass die Summe des neuen Kaufs größer als die Rückgabesumme [ist. Ermitteln Sie](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)vor dem Kauf die richtige Größe.
3.Überprüfen und Abschließen der Transaktion

**Rückerstattung für eine reservierte Instanz**

Um eine Reservierung zu erstatten, wechseln Sie zu **Reservierungsdetails,** und klicken Sie auf **Rückerstattung.**

**Anteilsgezahlte Rückerstattung:**

**Pro-rations- und Mindestanforderungsbeispiele für Rückerstattung und Austausch** Vorabreservierungsbeispiel:

- Sie erwerben am 1. Januar ein einjähriges Laufzeit-RI für 120 USD.
- Am 7. April möchten Sie diese Reservierung zurückerstatten oder umtauschen
- Da die Reservierung seit 97 Tagen live ist, erhalten Sie (1-97/365) * $120 zurück. (d. h. $88,1). Es gibt derzeit keine Strafen für Rückerstattungen
- Beim Austausch sollte Ihr neuer Kauf größer als $88,1 sein.
- Derzeit gibt es keine Strafen für Rückerstattungen

**Abrechnungsplanreservierungsbeispiel:**

- Sie erwerben ein einjähriges Laufzeit-RI für 10 USD pro Monat
- Am 7. April möchten Sie diese Reservierung zurückerstatten oder umtauschen
- Da die letzte Zahlung 7 Tage erfolgt ist, erhalten Sie (1-7/31) * $10 zurück. (d. h. $7,74)
- Die zukünftigen stornierten Zahlungen sind $ 80. Es gibt derzeit keine Strafen für Rückerstattungen
- Durch diese Stornierung werden $87,74 von der Rückerstattungsgrenze von 50.000 USD abgezogen.
- Beim Austausch sollte der Gesamtwert des neuen Kaufs größer als $87,74 sein.

**Rechnung für den letzten Abrechnungszeitraum nicht angezeigt**

Es gibt einige mögliche Gründe, warum eine Rechnung nicht zu sehen ist:

- Sie haben einen monatlichen Guthabenbetrag mit Ihrem Abonnement, den Sie nicht überschritten haben, oder Sie haben eine kostenlose Testversion. Eine Rechnung wird nur generiert, wenn Sie Geld schulden
- Es ist weniger als 30 Tage nach dem Tag, an dem Sie Azure abonniert haben
- Die Rechnung wird noch nicht generiert. Warten bis zum Ende des Abrechnungszeitraums
- Wenn Sie nicht der Kontoadministrator sind, stehen Ihnen ältere Rechnungen möglicherweise nicht zur Verfügung.

**Laden Sie Ihre Rechnung aus dem Azure-Portal herunter (.pdf)**

- Wählen Sie Ihr Abonnement auf der [Seite Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) im Azure-Portal als Benutzer mit Zugriff [auf Rechnungen aus.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Auswählen **von Rechnungen**
- Klicken Sie auf **Rechnung herunterladen**, um eine Kopie Ihrer PDF-Rechnung anzuzeigen. Wenn es **"Nicht verfügbar"** heißt, finden Sie weitere Informationen unter Warum wird keine Rechnung für den [letzten Abrechnungszeitraum angezeigt?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Empfangen Ihrer Rechnung per E-Mail (.pdf)**

- Wählen Sie Ihr Abonnement auf der [Seite Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) aus. Klicken **Sie auf Rechnungen** und dann auf Meine Rechnung senden
- Klicken **Sie auf Opt-in,** und akzeptieren Sie die Bedingungen. Sie müssen sich für jedes Abonnement, das Sie besitzen, entscheiden.

Hinweis: Wenn Sie nach den Schritten keine E-Mail erhalten, stellen Sie sicher, dass Ihre E-Mail-Adresse in den Kommunikationseinstellungen [ihres Profils richtig ist.](https://account.windowsazure.com/profile)

**Laden Sie Ihre Nutzungsdaten aus dem Azure-Portal herunter.**

- Anmelden beim [Azure Account Center](https://account.windowsazure.com/Subscriptions) als [Kontoadministrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Wählen Sie das Abonnement aus, für das Sie die Rechnung und Nutzungsinformationen benötigen.
- Auswählen **des Abrechnungsverlaufs**
- Wählen **Sie Aktuelle Anweisung anzeigen aus,** um eine Schätzung Ihrer Gebühren zum Zeitpunkt der Schätzung zu sehen.
- Wählen **Sie Nutzung herunterladen** aus, um die täglichen Verwendungsdaten als CSV-Datei herunterzuladen. Wenn zwei Versionen verfügbar sind, laden Sie Version 2 herunter.

Weitere Fragen: [Besuchen Sie reservierte Instanz-Dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Empfohlene Dokumente**

- [Grundlagen der Abrechnung](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verstehen, wie der Rabatt für reservierte Instanzen angewendet wird](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Herunterladen oder Anzeigen Ihrer Azure-Abrechnungsrechnung und der täglichen Nutzungsdaten](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verstehen, wie der Rabatt für reservierte Instanzen angewendet wird](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verstehen der Verwendung der reservierten Instanz für Ihr Pay-As-You-Go-Abonnement](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verstehen der Verwendung der reservierten Instanz für Ihre Enterprise-Registrierung](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-Softwarekosten nicht in reservierten Instanzen enthalten](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reservierte Instanzen im Programm für den zentralen Cloudlösungsanbieter (CSP) des Partners](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)