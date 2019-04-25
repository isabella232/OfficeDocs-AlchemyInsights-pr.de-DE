---
title: 1491-Suche-nicht-Rückgabe-erwartete-Ergebnisse
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383834"
---
# <a name="content-search-not-returning-expected-results"></a>Die Inhaltssuche gibt keine erwarteten Ergebnisse zurück

Wenn Sie die Inhaltssuche im Office 365 Security & Compliance Center durchführen, werden möglicherweise unerwartete Suchergebnisse angezeigt. Berücksichtigen Sie die folgenden Aspekte, die sich auf Ihre Suchergebnisse auswirken können:

- **Inhaltsspeicherorte und Suchbedingungen**: Vergewissern Sie sich, dass Sie die richtigen inhaltsspeicherorte und Suchbedingungen ausgewählt haben. Wenn Sie eine große Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie Sie in mehrere Suchvorgänge aufteilen.

- **Teilweise indizierte Elemente**: [teilweise indizierte Elemente](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten. Teilweise indizierte Elemente aus Websites in SharePoint und OneDrive sind jedoch nicht in der Such Schätzung enthalten.

- **Such**Fehler: beim Durchsuchen einer hohen Anzahl von Postfächern (über 100.000 Postfächer) können Suchfehler mit Fehlercodes wie CS008-009 und CS012-002 angezeigt werden. Wiederholen Sie in diesem Fall die Suche nur für die fehlerhaften inhaltsspeicherorte. Weitere Informationen finden Sie in [diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
