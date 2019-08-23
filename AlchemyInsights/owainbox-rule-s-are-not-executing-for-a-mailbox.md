---
title: 1332 OWA-Postfachregel (n) werden nicht für ein Postfach ausgeführt
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555772"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="aa42a-102">Eine Posteingangsregel funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="aa42a-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="aa42a-103">Überprüfen Sie die folgenden Einstellungen in Outlook im Internet:</span><span class="sxs-lookup"><span data-stu-id="aa42a-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="aa42a-104">Eine Nachricht kann nur einmal automatisch basierend auf Posteingangsregeln umgeleitet, weitergeleitet oder beantwortet werden.</span><span class="sxs-lookup"><span data-stu-id="aa42a-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="aa42a-105">Eine Umleitungsregel (eine Posteingangsregel oder eine Nachrichtenfluss Regel, die auch als Transportregel bezeichnet wird) kann maximal zehn Weiterleitungs Empfänger zu einer Nachricht hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="aa42a-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="aa42a-106">Weitere Informationen finden Sie unter [Journal-, Transport-und Posteingangsregel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="aa42a-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="aa42a-107">Posteingangsregeln funktionieren nicht mit dem alternativen Journalpostfach.</span><span class="sxs-lookup"><span data-stu-id="aa42a-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="aa42a-108">Weitere Informationen zum alternativen Journalpostfach finden Sie unter [alternative Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="aa42a-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="aa42a-109">Um diese Probleme zu beheben, lesen Sie [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="aa42a-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="aa42a-110">Wenn die vorherigen Probleme nicht zutreffen, führen Sie den Diagnosebericht "Posteingangsregel" aus, bevor Sie das Problem an den Microsoft-Support eskalieren:</span><span class="sxs-lookup"><span data-stu-id="aa42a-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="aa42a-111">Öffnen Sie das Postfach in Outlook im Internet, und klicken Sie auf</span><span class="sxs-lookup"><span data-stu-id="aa42a-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="aa42a-112">**Einstellungen** > **alle Outlook-Einstellungen** > **-e-Mail-** > **Regeln**anzeigen.</span><span class="sxs-lookup"><span data-stu-id="aa42a-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="aa42a-113">Klicken Sie unten auf der Seite auf **Wenn Ihre Regeln nicht funktionieren klicken Sie hier, um einen Diagnosebericht zu erstellen**.</span><span class="sxs-lookup"><span data-stu-id="aa42a-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
