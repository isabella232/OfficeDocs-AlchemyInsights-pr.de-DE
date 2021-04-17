---
title: Warum ist die Schaltfläche Budget hinzufügen für mich deaktiviert?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822634"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Warum ist die Schaltfläche Budget hinzufügen für mich deaktiviert?

Zum Erstellen eines Budgets benötigen Sie eine der folgenden Berechtigungen:

- Verwaltungsgruppe, Abonnement, Ressourcengruppenbereiche
- Mitwirkender für die Kostenverwaltung
- Besitzer
- Contributor
- Nur Enterprise-Kunde: Registrierung, Abteilung, Kontobereiche
- Registrierungsadministrator (Budget auf Registrierungsbereich festlegen)
- Abteilungsadministrator (Budget auf Abteilungsbereich festlegen)
- Kontobesitzer (Budget auf Kontobereich festlegen)
- Nur moderne Kundenvereinbarung: Abrechnungskonto, Abrechnungsprofil, Bereiche des Abschnitts Rechnung
- Ersteller von Azure-Abonnements

**Ich habe ein Budget erstellt, als meine Kosten für den aktuellen Monat bereits über dem Budget waren. Warum habe ich keine Warnung erhalten?**  
Wenn Sie bereits einen bestimmten Kostenschwellenwert überschritten haben, wenn Sie ein Budget erstellen, wird die Warnung nicht ausgelöst. Sobald ein neuer Zyklus beginnt, wird die Warnung ausgelöst, wenn Sie den Schwellenwert überschreiten.

**Wann sollte ich erwarten, dass ich eine Warnung erhalte, nachdem ich einen meiner definierten Schwellenwerte für Budgetwarnungen überschritten habe?**  
Budgets werden alle 4 Stunden ausgewertet. Es dauert mindestens 8 Stunden, bis Nutzungsdaten das Budgetsystem erreichen. Vor diesem Grund kann es bis zu 12 Stunden dauern, bis Warnungen ausgelöst werden, nachdem Sie einen Schwellenwert überschritten haben.

**Warum ist die Schaltfläche Startdatum deaktiviert, wenn ich einen Monat oder einen Abrechnungsmonatszurücksetzungszeitraum auswähle?**  
Budgets werden am aktuellen Kalendermonat oder aktuellen Abrechnungszeitraum ausgerichtet (in dem Fall, in dem Abrechnungsmonat ausgewählt ist). Daher füllen wir diesen Wert vorab für Sie auf.

**Warum wird in der Budgeterstellungserfahrung kein Diagramm meiner Kosten angezeigt?**  
Wir benötigen mindestens 2 Monate Kostendaten, bevor wir ein Diagramm rendern können, um Sie bei der Erstellung von Budget zu unterstützen.

**Warum kann ich kein Budget für ein gerade erstelltes Abonnement festlegen?**  
Nach dem Erstellen eines Abonnements dauert die Datenverarbeitung 24 bis 48 Stunden, bevor sie ein Budget festlegen.

**Budget-API-Ressourcen**

- [Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Stellt Vorgänge zum Erstellen und Aktualisieren von Budgets bereit. Mithilfe der Budgets-API können Sie einen Budgetschwellenwert festlegen und mehrere Warnungen so konfigurieren, dass sie ausgelöst werden, wenn Sie diesen Schwellenwert erreichen. Warnungen können eine E-Mail oder eine Azure-Aktionsgruppe auslösen, um Automatisierungen durchzuführen. Hinweis: Die Filterung für diese API entspricht nicht der Abfrage-API-Filterung/-dimension.
- [Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Erstellen von Budgets mit höheren Kostenfilterfunktionen als v1. Die Filterung richtet sich nach dem Vertrag, der in unseren Abfrage- und Dimensions-APIs verwendet wird. Dies ist die empfohlene Budget-API, um vorwärts zu gehen.
- [Dimensionen](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Stellt Vorgänge zum Erhalten unterstützter Dimensionen für Ihre Verwendung unter einer Vielzahl von Bereich zur Auswahl. Mithilfe der Dimensions-API können Sie eine Liste von Dimensionen abrufen, die als Eingaben zum Generieren von Abfragen mit der Abfrage-API verwendet werden können.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Stellt Vorgänge zum Erhalten aggregierter Kosten- und Nutzungsdaten basierend auf der von Ihnen zur Verfügung ierten Abfrage zur Verfügung. Mit der Abfrage-API können Sie die gewünschte Filterung, Sortierung und Gruppierung für alle verfügbaren Dimensionen angeben (auf die über die Dimensions-API zugegriffen wird).

**Prognostizierte Kosten**

**Warum werden in der Kostenanalyse keine Prognosen für meine Kosten sehen?**  
Es gibt mehrere Gründe, warum die Prognoseprojektion für Sie in der Kostenanalyse fehlt. Einige davon sind wie folgt:

1. Wenn Ihre Kostendaten weniger als 10 Tage alt sind, wird das Prognosediagramm nicht geladen. Das Modell benötigt mindestens 10 Tage neuer Kostendaten für genaue Projektionen.
2. Wenn Sie historische Datumsangaben ausgewählt haben, ist das Prognosediagramm nicht sichtbar. Wählen Sie einen Datumsbereich mit zukünftigen Datumsangaben für das prognosediagramm aus, das angezeigt werden soll.
3. Wenn Ihr Konto über mehrere Währungen verfügt, werden im Prognosediagramm nur Kosten für "Alle Kosten in USD" projiziert.

**Warum ändert sich die Prognose nicht, wenn ich Änderungen an meinen Ressourcen vorn nne?**  
Das Prognosemodell benötigt ein paar Tage, um Änderungen am Konto zu berücksichtigen, und es werden keine unmittelbaren Projektionen basierend auf der Änderung der Ressourcen vorgenommen.  
Bei größeren Schritten zur Erhöhung oder Verringerung der Ressourcen dauert es etwas länger, bis das Modell an diese Änderungen angepasst wird, um Anomalien zu berücksichtigen.

**Warum erhöht sich meine Prognose, nachdem ich eine Reservierung oder einen Marketplace-Kauf gemacht habe?**  
Das Prognosemodell berücksichtigt Ihre "Tatsächlichen Kosten" und berücksichtigt nicht die Verwendung und den Kauf separat. Bei einem Einmalkauf verringert das Modell die Projektionen nach 10 Tagen, um den plötzlichen Kostenanstieg zu berücksichtigen.

**Ich möchte Prognosen für eine einzelne Dimension (z. B. Meter)**  
Die Prognose unterstützt derzeit Die Gesamtkostenprojektionen und nicht für einzelne Zähler. Wenn also eine Dimension "nach" gruppierend ist, werden die Projektionen für die Gesamtzahl aller Elemente in der Dimension verwendet.

**Empfohlene Dokumente**

- [Was ist Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für azure cost management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysieren Ihrer Kosten und Ausgaben](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Untersuchen und Analysieren von Kosten mit Kostenanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Preise](https://azure.microsoft.com/services/cost-management/#pricing)
- [Überprüfen der Kosten in der Kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video-Lernprogramm: Erstellen eines Budgets im Azure-Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Voraussetzungen für das Anzeigen und Anpassen von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Erstellen und Verwalten von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurieren der Automatisierung mit der Azure Action Groups and Budgets-API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Verwenden von Kostenwarnungen zum Überwachen von Nutzung und Ausgaben](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für das Kostenmanagement](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Lernprogrammvideos**

- [Erstellen eines Budgets im Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Verwalten von Kosten mit der Budgets-API und Aktionsgruppen](https://go.microsoft.com/fwlink/?linkid=2147038)