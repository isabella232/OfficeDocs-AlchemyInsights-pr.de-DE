---
title: 1491-Suche-nicht-zurückgeben-erwartete-Ergebnisse
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709226"
---
# <a name="content-search-not-returning-expected-results"></a>Inhaltssuche gibt keine erwarteten Ergebnisse zurück

Wenn Sie Inhalts suchen im Microsoft 365 Security & Compliance Center durchführen, erhalten Sie möglicherweise unerwartete Suchergebnisse. Beachten Sie die folgenden Aspekte, die sich auf Ihre Suchergebnisse auswirken können:

- **Inhaltsspeicherorte und Suchbedingungen**: Stellen Sie sicher, dass Sie die richtigen inhaltsspeicherorte und Suchbedingungen ausgewählt haben. Wenn Sie eine große Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie Sie in mehrere Suchvorgänge aufteilen.

- **Teilweise indizierte Elemente**: [teilweise indizierte Elemente](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten. Teilweise indizierte Elemente aus Websites in SharePoint und OneDrive sind jedoch nicht in der Such Schätzung enthalten.

- **Suchfehler**: beim Durchsuchen einer großen Anzahl von Postfächern (über 100.000 Postfächer) erhalten Sie möglicherweise Suchfehler mit Fehlercodes wie CS008-009 und CS012-002. Wiederholen Sie in diesem Fall die Suche nur nach den fehlgeschlagenen Inhaltsspeicherorten. Weitere Informationen finden Sie in [diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
