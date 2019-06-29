---
title: 1491-Suche-nicht-zurückgeben-erwartete-Ergebnisse
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355876"
---
# <a name="content-search-not-returning-expected-results"></a>Inhaltssuche gibt keine erwarteten Ergebnisse zurück

Wenn Sie Inhalts suchen im Office 365 Security #a0 Compliance Center durchführen, erhalten Sie möglicherweise unerwartete Suchergebnisse. Beachten Sie die folgenden Aspekte, die sich auf Ihre Suchergebnisse auswirken können:

- **Inhaltsspeicherorte und Suchbedingungen**: Stellen Sie sicher, dass Sie die richtigen inhaltsspeicherorte und Suchbedingungen ausgewählt haben. Wenn Sie eine große Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie Sie in mehrere Suchvorgänge aufteilen.

- **Teilweise indizierte Elemente**: [teilweise indizierte Elemente](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten. Teilweise indizierte Elemente aus Websites in SharePoint und OneDrive sind jedoch nicht in der Such Schätzung enthalten.

- **Suchfehler**: beim Durchsuchen einer großen Anzahl von Postfächern (über 100.000 Postfächer) erhalten Sie möglicherweise Suchfehler mit Fehlercodes wie CS008-009 und CS012-002. Wiederholen Sie in diesem Fall die Suche nur nach den fehlgeschlagenen Inhaltsspeicherorten. Weitere Informationen finden Sie in [diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
