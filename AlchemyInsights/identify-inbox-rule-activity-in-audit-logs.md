---
title: Identifizieren von Posteingangsregel Aktivitäten in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909242"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2a4a0-102">Identifizieren von Posteingangsregel Aktivitäten in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="2a4a0-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2a4a0-103">Sie können die Überwachungsprotokoll Suche im Security & Compliance Center verwenden, um Posteingangsregel Ereignisse anzuzeigen (erstellen, ändern und Löschen von Posteingangsregeln).</span><span class="sxs-lookup"><span data-stu-id="2a4a0-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2a4a0-104">Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="2a4a0-105">Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="2a4a0-106">Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="2a4a0-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2a4a0-107">Überprüfen Sie unter **Exchange-Postfachaktivitäten**, ob das Feld **Aktivitäten** auf **New-InboxRule erstellen/ändern/aktivieren/deaktivieren**der Posteingangsregel festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2a4a0-108">Klicken Sie auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-108">Click **Search**.</span></span>

<span data-ttu-id="2a4a0-109">Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-109">In the results, select an audit record.</span></span> <span data-ttu-id="2a4a0-110">Klicken Sie im Detail Flyout auf **Weitere Informationen**.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2a4a0-111">Informationen zu den Einstellungen für die Posteingangsregel werden im Feld **Parameter** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2a4a0-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2a4a0-112">Weitere Informationen finden Sie unter [ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .</span><span class="sxs-lookup"><span data-stu-id="2a4a0-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
