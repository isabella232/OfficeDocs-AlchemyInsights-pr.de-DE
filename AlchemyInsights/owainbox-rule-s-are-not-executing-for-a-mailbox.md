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
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762222"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="5d746-102">Eine Posteingangsregel funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="5d746-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="5d746-103">Überprüfen Sie die folgenden Einstellungen:</span><span class="sxs-lookup"><span data-stu-id="5d746-103">Verify the following settings:</span></span>

- <span data-ttu-id="5d746-104">Eine Nachricht kann nur einmal automatisch basierend auf Posteingangsregeln umgeleitet, weitergeleitet oder beantwortet werden.</span><span class="sxs-lookup"><span data-stu-id="5d746-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="5d746-105">Eine Umleitungsregel (eine Posteingangsregel oder eine Nachrichtenfluss Regel, die auch als Transportregel bezeichnet wird) kann maximal zehn Weiterleitungs Empfänger zu einer Nachricht hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="5d746-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="5d746-106">Weitere Informationen finden Sie unter [Journal-, Transport-und Posteingangsregel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="5d746-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="5d746-107">Posteingangsregeln funktionieren nicht mit dem alternativen Journalpostfach.</span><span class="sxs-lookup"><span data-stu-id="5d746-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="5d746-108">Weitere Informationen zum alternativen Journalpostfach finden Sie unter [alternative Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5d746-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="5d746-109">Um diese Probleme zu beheben, lesen Sie [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="5d746-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="5d746-110">Wenn die vorherigen Probleme nicht zutreffen, führen Sie den Diagnosebericht "Posteingangsregel" aus, bevor Sie das Problem an den Microsoft-Support eskalieren:</span><span class="sxs-lookup"><span data-stu-id="5d746-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="5d746-111">Öffnen Sie das Postfach in Outlook im Internet, und klicken Sie auf **Einstellungen** \> **Optionen** \> **e-Mail-** \> **Posteingangsregeln**organisieren.</span><span class="sxs-lookup"><span data-stu-id="5d746-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="5d746-112">Klicken Sie unten auf der Seite auf **Wenn Ihre Regeln nicht funktionieren klicken Sie hier, um einen Diagnosebericht zu erstellen**.</span><span class="sxs-lookup"><span data-stu-id="5d746-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
