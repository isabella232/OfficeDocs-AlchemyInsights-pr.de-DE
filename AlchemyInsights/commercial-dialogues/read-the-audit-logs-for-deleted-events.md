---
title: Lesen der Überwachungsprotokolle für gelöschte Ereignisse
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464603"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="d8be6-102">Lesen der Überwachungsprotokolle für gelöschte Ereignisse</span><span class="sxs-lookup"><span data-stu-id="d8be6-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="d8be6-103">Hier erfahren Sie, wie Sie dies tun:</span><span class="sxs-lookup"><span data-stu-id="d8be6-103">Here's how to do this:</span></span>

1. <span data-ttu-id="d8be6-104">Wechseln Sie zum [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="d8be6-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="d8be6-105">Wählen **Sie Suche**  >  [**Überwachungsprotokollsuche aus.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="d8be6-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="d8be6-106">Wenn Sie eine Benachrichtigung sehen, dass Sie das Feature aktivieren müssen, fahren Sie mit dem Feature voran, und aktivieren Sie es jetzt.</span><span class="sxs-lookup"><span data-stu-id="d8be6-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="d8be6-107">Wenn das Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben ziehen.</span><span class="sxs-lookup"><span data-stu-id="d8be6-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="d8be6-108">Wählen **Sie Aktivitäten** aus, und suchen Sie dann nach **Exchange-Postfachaktivitäten.**</span><span class="sxs-lookup"><span data-stu-id="d8be6-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="d8be6-109">Wählen Sie **die Ordneroptionen Gelöschte Nachrichten** aus dem Ordner Gelöschte Elemente und **In Gelöschte Elemente** verschobene Nachrichten aus.</span><span class="sxs-lookup"><span data-stu-id="d8be6-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="d8be6-110">Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den Bereich **Aktivitäten zu** minimieren.</span><span class="sxs-lookup"><span data-stu-id="d8be6-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="d8be6-111">Geben Sie den Datumsbereich an, und wählen Sie dann im Feld **Benutzer** den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten.</span><span class="sxs-lookup"><span data-stu-id="d8be6-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="d8be6-112">Sie können mehrere Benutzer gleichzeitig auswählen.</span><span class="sxs-lookup"><span data-stu-id="d8be6-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="d8be6-113">Wählen Sie **Suchen aus.**</span><span class="sxs-lookup"><span data-stu-id="d8be6-113">Select **Search**.</span></span> <span data-ttu-id="d8be6-114">Die Aktivitäten werden unter **Ergebnisse angezeigt.**</span><span class="sxs-lookup"><span data-stu-id="d8be6-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="d8be6-115">Wählen Sie zum Anzeigen der Details eine Aktivität aus, und wählen Sie dann **Weitere Informationen aus.**</span><span class="sxs-lookup"><span data-stu-id="d8be6-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="d8be6-116">Zusätzliche Informationen zum gelöschten Element, z. B. die Betreffzeile und der Speicherort des Elements, wenn es gelöscht wurde, werden im **Feld AffectedItems** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d8be6-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="d8be6-117">Gelöschte Elemente können nicht mithilfe des Überwachungsprotokollfeatures wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="d8be6-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="d8be6-118">Informationen zum Wiederherstellen gelöschter Elemente finden Sie unter [Wiederherstellen gelöschter Elemente oder E-Mails in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="d8be6-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="d8be6-119">Weitere Informationen finden Sie unter [Durchsuchen des Office 365-Überwachungsprotokolls zur Problembehandlung gängiger Szenarien.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="d8be6-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
