---
title: Warum ist die Schaltfläche "Budget hinzufügen" für mich deaktiviert?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769589"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Warum ist die Schaltfläche "Budget hinzufügen" für mich deaktiviert?

Um ein Budget zu erstellen, benötigen Sie eine der folgenden Berechtigungen:

- Verwaltungsgruppen-, Abonnement-, Ressourcengruppen Bereiche
- Kosten Management Mitwirkender
- Besitzer
- Contributor
- Nur Enterprise-Kunde: Registrierung, Abteilung, Kontobereiche
- Registrierungs Administrator (Budget im Registrierungsbereich festlegen)
- Abteilungsadministrator (Budget im Abteilungsbereich festlegen)
- Kontobesitzer (Budget unter Kontobereich festlegen)
- Nur moderne Kundenvereinbarung: Abrechnungskonto, Abrechnungsprofil, Rechnungs Bereichs Bereiche
- Azure Subscription Creator

**Ich habe ein Budget erstellt, wenn meine Kosten für den aktuellen Monat bereits über dem Budget liegen. Warum habe ich keine Benachrichtigung erhalten?**  
Wenn Sie bereits einen bestimmten Kosten Schwellenwert überschritten haben, wenn Sie ein Budget erstellen, wird keine Warnung ausgelöst. Wenn ein neuer Zyklus beginnt, wenn Sie den Schwellenwert verletzen, wird die Warnung ausgelöst.

**Wann sollte ich erwarten, dass eine Warnung angezeigt wird, nachdem ich eine der definierten Schwellenwerte für den Budget Alarm überschritten habe?**  
Die Budgets werden alle vier Stunden ausgewertet. Es dauert mindestens 8 Stunden, bis die Verwendungsdaten das Budget System erreichen. In diesem Fall kann es bis zu 12 Stunden dauern, bis nach Überschreitung eines Schwellenwerts eine Warnung ausgelöst wird.

**Warum ist die Schaltfläche "Start Datum" deaktiviert, wenn ich einen Monat oder einen Abrechnungsmonat für den zurück setzungs Zeitraum wähle?**  
Die Budgets werden an den aktuellen Kalendermonat oder den aktuellen Abrechnungszeitraum angepasst (im Fall, in dem der Abrechnungsmonat ausgewählt ist). Daher wird dieser Wert für Sie vorab aufgefüllt.

**Warum wird in der Budget Erstellungsumgebung kein Diagramm meiner Kosten angezeigt?**  
Wir benötigen mindestens 2 Monate Kostendaten, bevor wir einen Graphen Rendern können, um Sie bei der Erstellung von Budgets zu unterstützen.

**Warum kann ich kein Budget für ein soeben erstelltes Abonnement festlegen?**  
Nach dem Erstellen eines Abonnements dauert die Verarbeitung der Daten 24-48 Stunden, bevor ein Budget dafür festgesetzt wird.

**Ressourcen für die Budget-API**

- [Budgets-API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): stellt Vorgänge zum Erstellen und Aktualisieren von Budgets bereit. Mithilfe der Budgets-API können Sie einen Schwellenwert für das Budget festlegen und mehrere Warnungen so konfigurieren, dass Sie beim Erreichen dieses Schwellenwerts ausgelöst werden. Benachrichtigungen können eine e-Mail oder eine Azure-Aktionsgruppe auslösen, um Automatisierung auszuführen. Hinweis: das Filtern für diese API wird nicht mit der Abfrage-API-Filterung/den Dimensionen ausgerichtet.
- [Budgets-API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Erstellen von Budgets mit mehr Kosten Filterungsfunktionen als v1. Das Filtern wird an dem in unseren Abfrage-und Dimensions-APIs verwendeten Vertrag ausgerichtet. Dies ist die empfohlene Budgets-API für die Verwendung von Moving Forward.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): stellt Vorgänge bereit, um unterstützte Dimensionen für ihre Verwendung unter einer Vielzahl von Bereichen zu erhalten. Mithilfe der Dimensions-API können Sie eine Liste von Dimensionen abrufen, die als Eingaben zum Generieren von Abfragen mit der Abfrage-API verwendet werden können.
- [Abfrage](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): stellt Vorgänge bereit, um aggregierte Kosten und Nutzungsdaten basierend auf der von Ihnen bereitgestellten Abfrage abzurufen. Mithilfe der Abfrage-API können Sie die gewünschte Filterung, Sortierung und Gruppierung für alle verfügbaren Dimensionen angeben (auf die über die Dimensions-API zugegriffen wird).

**Prognostizierte Kosten**

**Warum werden Prognosen für meine Kosten in der Kostenanalyse nicht angezeigt?**  
Es gibt mehrere Gründe, warum die Prognose Projektion in der Kostenanalyse möglicherweise fehlt, einige davon lauten wie folgt:

1. Wenn Ihre Kostendaten weniger als 10 Tage alt sind, wird das Prognose Diagramm nicht belastet. Das Modell benötigt mindestens 10 Tage der aktuellen Kostendaten für genaue Projektionen
2. Wenn Sie historische Datumsangaben ausgewählt haben, ist das Prognose Diagramm nicht sichtbar. Wählen Sie einen Datumsbereich mit zukünftigen Datumsangaben für das angezeigte Prognose Diagramm aus.
3. Wenn Ihr Konto über mehrere Währungen verfügt, projiziert das Prognose Diagramm nur Kosten für ' alle Kosten in USD '.

**Warum ändert sich die Prognose nicht, wenn ich Änderungen an meinen Ressourcen vorgenommen habe?**  
Das Prognosemodell erfordert einige Tage, um Änderungen im Konto zu berücksichtigen, und es werden keine unmittelbaren Projektionen basierend auf der Änderung der Ressourcen vorgenommen.  
Für größere Schritte beim Vergrößern oder Verkleinern von Ressourcen dauert es etwas länger, bis das Modell sich an diese Änderungen angepasst hat, um Anomalien zu berücksichtigen.

**Warum steigt meine Prognose an, nachdem ich eine Reservierung getätigt oder den Kauf eines Marktplatzes vorgenommen habe?**  
Das Prognosemodell berücksichtigt Ihre "tatsächlichen Kosten" und berücksichtigt nicht die Verwendung und den Kauf separat. Für einen einmaligen Einkauf verringert das Modell die Projektionen nach 10 Tagen, um den plötzlichen Anstieg der Kosten zu berücksichtigen.

**Ich möchte Prognosen für eine einzelne Dimension anzeigen (zB. Meter**  
Prognose unterstützt derzeit Gesamtkosten Projektionen und nicht für einzelne Zähler. Wenn also "gruppiert nach" eine Dimension ist, werden die Projektionen für die Summe aller Elemente in der Dimension

**Empfohlene Dokumente**

- [Was ist Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysieren ihrer Kosten und Ausgaben](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Untersuchen und Analysieren von Kosten mit Kostenanalysen](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Preise](https://azure.microsoft.com/services/cost-management/#pricing)
- [Überprüfen der Kosten in der Kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video Lernprogramm: Erstellen eines Budgets im Azure-Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Voraussetzungen für das Anzeigen und Anpassen von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Erstellen und Verwalten von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurieren der Automatisierung mit Azure Action Groups und Budgets API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Verwenden von Kosten Warnungen zum Überwachen der Nutzung und Ausgaben](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für das Kosten Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Tutorial-Videos**

- [Erstellen eines Budgets im Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Verwalten von Kosten mit den Budgets-API-und Aktionsgruppen](https://go.microsoft.com/fwlink/?linkid=2147038)