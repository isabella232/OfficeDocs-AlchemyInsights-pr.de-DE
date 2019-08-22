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
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539166"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="22257-102">Identifizieren der Posteingangsregel Aktivität in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="22257-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="22257-103">Sie können die Überwachungsprotokoll Suche im Office 365 Security #a0 Compliance Center verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).</span><span class="sxs-lookup"><span data-stu-id="22257-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="22257-104">Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/)an.</span><span class="sxs-lookup"><span data-stu-id="22257-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="22257-105">Wechseln Sie zur \*\*\*\* > Suchseite**Überwachungsprotokoll** suchen.</span><span class="sxs-lookup"><span data-stu-id="22257-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="22257-106">Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="22257-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="22257-107">Stellen Sie sicher, dass unter **Exchange-Postfachaktivitäten**das Feld **Aktivitäten** auf **neu-InboxRule Create/Modify/Enable/Disable Posteingangsregel**festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="22257-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="22257-108">Klicken Sie auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="22257-108">Click **Search**.</span></span>

<span data-ttu-id="22257-109">Wählen Sie in den Ergebnissen einen Überwachungseintrag aus.</span><span class="sxs-lookup"><span data-stu-id="22257-109">In the results, select an audit record.</span></span> <span data-ttu-id="22257-110">Klicken Sie im Detail Flyout auf **Weitere Informationen**.</span><span class="sxs-lookup"><span data-stu-id="22257-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="22257-111">Im Feld **Parameter** werden Informationen zu den Einstellungen für Posteingangsregeln angezeigt.</span><span class="sxs-lookup"><span data-stu-id="22257-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="22257-112">Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) hat.</span><span class="sxs-lookup"><span data-stu-id="22257-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
