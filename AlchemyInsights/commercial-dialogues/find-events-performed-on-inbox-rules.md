---
title: Suchen von Ereignissen, die für Posteingangsregeln ausgeführt werden
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464703"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="1484c-102">Suchen von Ereignissen, die für Posteingangsregeln ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="1484c-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="1484c-103">Wenn Posteingangsregeln erstellt, geändert oder gelöscht werden, werden die Ereignisse im Überwachungsprotokoll aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="1484c-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="1484c-104">Hier erfahren Sie, wie Sie sie überprüfen:</span><span class="sxs-lookup"><span data-stu-id="1484c-104">Here's how to review them:</span></span>

1. <span data-ttu-id="1484c-105">Wechseln Sie zum [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="1484c-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="1484c-106">Wählen Sie Suchen > Überwachungsprotokollsuche aus.</span><span class="sxs-lookup"><span data-stu-id="1484c-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1484c-107">Wenn Sie eine Benachrichtigung sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie mit der Überwachung voran, und aktivieren Sie sie jetzt.</span><span class="sxs-lookup"><span data-stu-id="1484c-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="1484c-108">Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben ziehen.</span><span class="sxs-lookup"><span data-stu-id="1484c-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="1484c-109">Wählen Sie das Feld Aktivitäten aus, und suchen Sie nach Exchange-Postfachaktivitäten, und wählen Sie dann New-InboxRule Posteingangsregel in Outlook Web App erstellen aus.</span><span class="sxs-lookup"><span data-stu-id="1484c-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="1484c-110">Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den Bereich Aktivitäten zu minimieren.</span><span class="sxs-lookup"><span data-stu-id="1484c-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="1484c-111">Geben Sie den Datumsbereich an, und wählen Sie dann im Feld Benutzer den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten.</span><span class="sxs-lookup"><span data-stu-id="1484c-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="1484c-112">Sie können mehrere Benutzer gleichzeitig auswählen.</span><span class="sxs-lookup"><span data-stu-id="1484c-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="1484c-113">Wählen Sie Suchen aus.</span><span class="sxs-lookup"><span data-stu-id="1484c-113">Select Search.</span></span> <span data-ttu-id="1484c-114">Die Aktivitäten werden unter Ergebnisse angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1484c-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="1484c-115">Um Details anzuzeigen, wählen Sie eine Aktivität aus, und wählen Sie dann Weitere Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="1484c-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="1484c-116">Im Abschnitt Parameter sehen Sie den Namen der Regel, die festgelegten Bedingungen und die Aktionen, die die Regel ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="1484c-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="1484c-117">Weitere Informationen finden Sie unter Durchsuchen des Office 365-Überwachungsprotokolls zur Problembehandlung gängiger Szenarien.</span><span class="sxs-lookup"><span data-stu-id="1484c-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>