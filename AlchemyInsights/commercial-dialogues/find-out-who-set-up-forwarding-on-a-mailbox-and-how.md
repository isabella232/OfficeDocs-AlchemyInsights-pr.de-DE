---
title: Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464615"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="4f4d2-102">Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie</span><span class="sxs-lookup"><span data-stu-id="4f4d2-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="4f4d2-103">Wenn die externe Weiterleitung für ein Postfach festgelegt wurde, wird die Aktivität im Rahmen des cmdlets Set-Mailbox überwacht.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="4f4d2-104">So finden Sie die Aktivität im Überwachungsprotokoll:</span><span class="sxs-lookup"><span data-stu-id="4f4d2-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="4f4d2-105">Wechseln Sie zum [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="4f4d2-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="4f4d2-106">Wählen **Sie Suche** >  **Überwachungsprotokollsuche aus.**</span><span class="sxs-lookup"><span data-stu-id="4f4d2-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="4f4d2-107">Wenn Sie eine Benachrichtigung sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie mit der Überwachung voran, und aktivieren Sie sie jetzt.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="4f4d2-108">Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben ziehen.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="4f4d2-109">Stellen Sie **sicher, dass das** Feld Aktivitäten auf Ergebnisse für alle Aktivitäten anzeigen festgelegt ist (Standardeinstellung). </span><span class="sxs-lookup"><span data-stu-id="4f4d2-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="4f4d2-110">Geben Sie den Datumsbereich an.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-110">Specify the date range.</span></span> <span data-ttu-id="4f4d2-111">Sie müssen keinen Benutzernamen angeben.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="4f4d2-112">Wählen Sie **Suchen aus.**</span><span class="sxs-lookup"><span data-stu-id="4f4d2-112">Select **Search**.</span></span> <span data-ttu-id="4f4d2-113">Die Aktivitäten werden unter **Ergebnisse angezeigt.**</span><span class="sxs-lookup"><span data-stu-id="4f4d2-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="4f4d2-114">Wählen **Sie Ergebnisse filtern** aus, und geben Sie dann **Set-mailbox** in das Feld **Aktivitätsfilter** ein.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="4f4d2-115">Dadurch werden alle **Set-Mailbox-Aktivitäten** zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="4f4d2-116">Wählen Sie zum Anzeigen der Details eine Aktivität aus, und wählen Sie dann **Weitere Informationen aus.**</span><span class="sxs-lookup"><span data-stu-id="4f4d2-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="4f4d2-117">Unter **Parametern** wird die Weiterleitungs-E-Mail-Adresse angezeigt, die für das Postfach festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="4f4d2-118">Die **UserID** stellt den Benutzer dar, der die externe Weiterleitung für das Postfach eingerichtet hat.</span><span class="sxs-lookup"><span data-stu-id="4f4d2-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="4f4d2-119">Weitere Informationen finden Sie unter [Durchsuchen des Office 365-Überwachungsprotokolls zur Problembehandlung gängiger Szenarien.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="4f4d2-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>