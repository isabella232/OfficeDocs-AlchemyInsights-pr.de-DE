---
title: 1491-Search-NOT-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964863"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="7c42c-102">Inhaltssuche nicht die erwarteten Ergebnisse zurückgibt</span><span class="sxs-lookup"><span data-stu-id="7c42c-102">Content Search not returning expected results</span></span>

<span data-ttu-id="7c42c-p101">Wenn für die Ausführung Content-Suche über die Sicherheit in Office 365 & Compliance Center möglicherweise unerwartete Suchergebnisse angezeigt. Berücksichtigen Sie die folgenden Schritte aus, die die Suchergebnisse beeinflussen:</span><span class="sxs-lookup"><span data-stu-id="7c42c-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="7c42c-p102">**Speicherorte für Inhalte und Suchkriterien**: Stellen Sie sicher, dass Sie die entsprechenden Speicherorte für Inhalte ausgewählt haben, und Suchen von Bedingungen. Wenn Sie eine große Suche (mit vielen Standorten) ausgeführt haben, sollten Sie es auf mehrere Suchvorgänge aufteilen.</span><span class="sxs-lookup"><span data-stu-id="7c42c-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="7c42c-p103">**Teilweise indizierte Elemente**: [teilweise indizierte Elemente](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) von Postfächern in der geschätzten Suchergebnisse enthalten sind. Allerdings werden nicht teilweise indizierte Elemente von Websites in SharePoint und OneDrive in die Schätzung für das Search enthalten.</span><span class="sxs-lookup"><span data-stu-id="7c42c-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="7c42c-p104">**Search-Fehler**: bei der Suche einer großen Anzahl von Postfächern (über 100.000 Postfächern) erhalten Sie möglicherweise Search-Fehler mit Fehlercodes wie CS008-009 und CS012-002). In diesem Fall wiederholen Sie die Suche nur für die fehlgeschlagene Speicherorte für Inhalte. [In diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) finden Sie weitere Informationen finden.</span><span class="sxs-lookup"><span data-stu-id="7c42c-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
