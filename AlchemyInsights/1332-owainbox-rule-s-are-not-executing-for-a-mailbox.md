---
title: 1332 OWA - Posteingang Regeln nicht für ein Postfach ausgeführt werden
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470429"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="8c7e6-102">Eine Posteingangsregel funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="8c7e6-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="8c7e6-103">Überprüfen Sie die folgenden Einstellungen:</span><span class="sxs-lookup"><span data-stu-id="8c7e6-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="8c7e6-p101">Eine Nachricht kann weitergeleitete oder beantwortete automatisch basierend auf Posteingangsregeln nur einmal umgeleitet werden. Eine umleiten Regel (Posteingangsregel oder e-Mail-Flussregel, auch bekannt als eine Transportregel) kann maximal 10 Weiterleitung der Empfänger einer Nachricht hinzufügen. Weitere Informationen finden Sie unter [Journal, Transport, und Posteingang Regel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="8c7e6-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="8c7e6-p102">Posteingangsregeln funktionieren nicht auf die alternatives Journalpostfach. Weitere Informationen zu den alternatives Journalpostfach finden Sie unter [alternatives Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="8c7e6-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="8c7e6-109">Zum Beheben dieser Probleme finden Sie unter [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="8c7e6-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="8c7e6-110">Wenn die vorherigen Problemen nicht angewendet werden, führen Sie den Posteingang Regel Diagnosebericht, bevor Sie das Problem an Microsoft Support ausweiten:</span><span class="sxs-lookup"><span data-stu-id="8c7e6-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="8c7e6-111">Öffnen Sie das Postfach in Outlook im Web, und klicken Sie auf **Einstellungen** \> **Optionen** \> **Organisieren e-Mail** \> **Posteingangsregeln**.</span><span class="sxs-lookup"><span data-stu-id="8c7e6-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="8c7e6-112">Klicken Sie am unteren Rand der Seite **Wenn Ihre Regeln klicken Sie hier, um einen Diagnosebericht generieren nicht funktionieren**.</span><span class="sxs-lookup"><span data-stu-id="8c7e6-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

