---
title: Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755037"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="83a82-102">Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="83a82-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="83a82-103">Sie können die Überwachungsprotokoll Suche im Security #a0 Compliance Center verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).</span><span class="sxs-lookup"><span data-stu-id="83a82-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="83a82-104">Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.</span><span class="sxs-lookup"><span data-stu-id="83a82-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="83a82-105">Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.</span><span class="sxs-lookup"><span data-stu-id="83a82-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="83a82-106">Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="83a82-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="83a82-107">Stellen Sie sicher, dass unter **Exchange-Postfachaktivitäten**das Feld **Aktivitäten** auf **neu-InboxRule Create/Modify/Enable/Disable Posteingangsregel**festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="83a82-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="83a82-108">Klicken Sie auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="83a82-108">Click **Search**.</span></span>

<span data-ttu-id="83a82-109">Wählen Sie in den Ergebnissen einen Überwachungseintrag aus.</span><span class="sxs-lookup"><span data-stu-id="83a82-109">In the results, select an audit record.</span></span> <span data-ttu-id="83a82-110">Klicken Sie im Detail Flyout auf **Weitere Informationen**.</span><span class="sxs-lookup"><span data-stu-id="83a82-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="83a82-111">Im Feld **Parameter** werden Informationen zu den Einstellungen für Posteingangsregeln angezeigt.</span><span class="sxs-lookup"><span data-stu-id="83a82-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="83a82-112">Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) hat.</span><span class="sxs-lookup"><span data-stu-id="83a82-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
