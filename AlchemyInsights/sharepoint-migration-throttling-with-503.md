---
title: SharePoint-Migrations Einschränkung mit 503 Fehlern
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931657"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>SharePoint-Migrations Einschränkung mit 503 Fehlern

**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird. Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen. In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.

Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt. Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen. Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.

**503 Fehler beim Migrieren zu SharePoint Online**

Es wird angezeigt, dass Sie zu SharePoint Online und empfangen von 503-Fehlern migrieren. Führen Sie die folgenden Schritte aus, damit wir Ihnen so schnell wie möglich behilflich sein können. 

1. Klicken Sie auf **Kontakt Support**und dann auf **Neue Dienstanforderung**.
2. Geben Sie für den Titel und die Beschreibung **SharePoint-Migrations Einschränkung mit 503**ein.
3. Sobald das Ticket übermittelt wurde, aktualisieren Sie es mit den folgenden Informationen:
    - Wie viel Links von der Migration (zum Beispiel, wie viele TBS?).
    - Migrations Start-und-Enddatum.
    - Beschreiben Sie, wo Sie Ihre Inhalte migrieren, beispielsweise SharePoint Server, Box, GDrive, Dateifreigaben usw.
    - Schätzen Sie die Anzahl der Einschränkungsfehler (beispielsweise x-Drosselung pro Stunde?) und wann ist die Drosselung aufgetreten.
    - Welches Migrationstool Sie verwenden (beispielsweise SPMT oder ShareGate).


