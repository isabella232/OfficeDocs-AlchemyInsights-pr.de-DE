---
title: Anwenden bewährter Methoden für erweiterte Suchabfragen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568622"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Anwenden bewährter Methoden für erweiterte Suchabfragen

Wenden Sie die folgenden bewährten Methoden an, um ergebnisse schneller zu erzielen und Timeouts beim Ausführen komplexer Abfragen zu vermeiden:

- Verwenden Sie beim Ausprobieren neuer Abfragen immer einen Grenzwert, um extrem große Ergebnissätze zu vermeiden. Verwenden Sie außerdem, um eine erste Bewertung der Größe des `count` Ergebnissatzs zu erstellen.
- Verwenden Sie zunächst Zeitfilter. Im Idealfall beschränken Sie Ihre Abfragen auf sieben Tage.
- Fügen Sie am Anfang einer Abfrage direkt nach dem Zeitfilter die Filter hinzu, von der erwartet wird, dass die meisten Daten entfernt werden.
- Wenn Sie nach vollständigen Token suchen, verwenden Sie den `has` Operator anstelle von `contains` .
- Führen Sie eine Suche für eine bestimmte Spalte und nicht für alle Spalten aus.
- Geben Sie beim Verknüpfen von Tabellen zunächst die Tabelle mit weniger Zeilen an.
- `project` nur die erforderlichen Spalten aus den Tabellen, die Sie beigetreten haben.

Weitere Informationen finden Sie unter Bewährte Methoden [für erweiterte Suchabfragen.](https://go.microsoft.com/fwlink/?linkid=2144812)
