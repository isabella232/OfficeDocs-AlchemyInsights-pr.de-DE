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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736856"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="9f7df-102">Anwenden bewährter Methoden für erweiterte Suchabfragen</span><span class="sxs-lookup"><span data-stu-id="9f7df-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="9f7df-103">Wenden Sie die folgenden bewährten Methoden an, um ergebnisse schneller zu erzielen und Timeouts beim Ausführen komplexer Abfragen zu vermeiden:</span><span class="sxs-lookup"><span data-stu-id="9f7df-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="9f7df-104">Verwenden Sie beim Ausprobieren neuer Abfragen immer einen Grenzwert, um extrem große Ergebnissätze zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="9f7df-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="9f7df-105">Verwenden Sie außerdem, um eine erste Bewertung der Größe des `count` Ergebnissatzs zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="9f7df-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="9f7df-106">Verwenden Sie zunächst Zeitfilter.</span><span class="sxs-lookup"><span data-stu-id="9f7df-106">Use time filters first.</span></span> <span data-ttu-id="9f7df-107">Im Idealfall beschränken Sie Ihre Abfragen auf sieben Tage.</span><span class="sxs-lookup"><span data-stu-id="9f7df-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="9f7df-108">Fügen Sie am Anfang einer Abfrage direkt nach dem Zeitfilter die Filter hinzu, von der erwartet wird, dass die meisten Daten entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="9f7df-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="9f7df-109">Wenn Sie nach vollständigen Token suchen, verwenden Sie den `has` Operator anstelle von `contains` .</span><span class="sxs-lookup"><span data-stu-id="9f7df-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="9f7df-110">Führen Sie eine Suche für eine bestimmte Spalte und nicht für alle Spalten aus.</span><span class="sxs-lookup"><span data-stu-id="9f7df-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="9f7df-111">Geben Sie beim Verknüpfen von Tabellen zunächst die Tabelle mit weniger Zeilen an.</span><span class="sxs-lookup"><span data-stu-id="9f7df-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="9f7df-112">`project` nur die erforderlichen Spalten aus den Tabellen, die Sie beigetreten haben.</span><span class="sxs-lookup"><span data-stu-id="9f7df-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="9f7df-113">Weitere Informationen finden Sie unter Bewährte Methoden [für erweiterte Suchabfragen.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="9f7df-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
