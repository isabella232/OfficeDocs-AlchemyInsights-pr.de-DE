---
title: 1490-Troubleshooting-eDiscovery-Failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277831"
---
# <a name="troubleshoot-content-search-errors"></a>Beheben von Fehlern bei der Inhaltssuche

Treten beim Exportieren von Suchergebnissen Probleme bei der Inhaltssuche oder beim Ermitteln von Fehlern auf?

Erhalten Sie beispielsweise beim Ausführen von Suchvorgängen Folgendes?

- CS008-oder CS012-Fehler

- Server beschäftigt/Timeoutfehler

- Anwendungsfehler aufgetreten

Oder erhalten Sie beim Suchen oder Exportieren von Ergebnissen aus einer großen Anzahl von Postfächern (über 100.000 Postfächern) Exportfehler?

Wiederholen Sie bei diesen Fehlertypen die Suche nach den fehlerhaften Inhaltsspeicherorten. Weitere Informationen finden Sie in  [diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Wenn Sie mehr als 100K-Postfächer exportieren, müssen Sie die folgenden PowerShell verwenden, um die Exportergebnisse herunterzuladen:  [Exportieren von Ergebnissen aus mehr als 100K Postfächern](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
