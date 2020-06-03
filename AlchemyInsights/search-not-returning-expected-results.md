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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510571"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="eecb0-102">Inhaltssuche gibt keine erwarteten Ergebnisse zurück</span><span class="sxs-lookup"><span data-stu-id="eecb0-102">Content Search not returning expected results</span></span>

<span data-ttu-id="eecb0-103">Wenn Sie Inhalts suchen im Microsoft 365 Security & Compliance Center durchführen, erhalten Sie möglicherweise unerwartete Suchergebnisse.</span><span class="sxs-lookup"><span data-stu-id="eecb0-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="eecb0-104">Beachten Sie die folgenden Aspekte, die sich auf Ihre Suchergebnisse auswirken können:</span><span class="sxs-lookup"><span data-stu-id="eecb0-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="eecb0-105">**Inhaltsspeicherorte und Suchbedingungen**: Stellen Sie sicher, dass Sie die richtigen inhaltsspeicherorte und Suchbedingungen ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="eecb0-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="eecb0-106">Wenn Sie eine große Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie Sie in mehrere Suchvorgänge aufteilen.</span><span class="sxs-lookup"><span data-stu-id="eecb0-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="eecb0-107">**Teilweise indizierte Elemente**: [teilweise indizierte Elemente](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten.</span><span class="sxs-lookup"><span data-stu-id="eecb0-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="eecb0-108">Teilweise indizierte Elemente aus Websites in SharePoint und OneDrive sind jedoch nicht in der Such Schätzung enthalten.</span><span class="sxs-lookup"><span data-stu-id="eecb0-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="eecb0-109">**Suchfehler**: beim Durchsuchen einer großen Anzahl von Postfächern (über 100.000 Postfächer) erhalten Sie möglicherweise Suchfehler mit Fehlercodes wie CS008-009 und CS012-002.</span><span class="sxs-lookup"><span data-stu-id="eecb0-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="eecb0-110">Wiederholen Sie in diesem Fall die Suche nur nach den fehlgeschlagenen Inhaltsspeicherorten.</span><span class="sxs-lookup"><span data-stu-id="eecb0-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="eecb0-111">Weitere Informationen finden Sie in [diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="eecb0-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
