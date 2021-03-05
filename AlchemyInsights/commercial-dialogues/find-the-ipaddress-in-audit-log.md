---
title: Suchen der IP-Adresse im Überwachungsprotokoll
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464704"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="f03fb-102">Suchen der IP-Adresse im Überwachungsprotokoll</span><span class="sxs-lookup"><span data-stu-id="f03fb-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="f03fb-103">Die IP-Adresse, die einer Aktivität eines Benutzers oder Administrators entspricht, wird in den Überwachungsprotokollen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f03fb-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="f03fb-104">Die Clientinformationen werden ebenfalls protokolliert.</span><span class="sxs-lookup"><span data-stu-id="f03fb-104">The client information is also logged.</span></span> <span data-ttu-id="f03fb-105">So identifizieren Sie die IP-Adresse:</span><span class="sxs-lookup"><span data-stu-id="f03fb-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="f03fb-106">Wechseln Sie zum [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="f03fb-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f03fb-107">Wählen **Sie Suche**  >  **[Überwachungsprotokollsuche aus.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="f03fb-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f03fb-108">Wenn Sie eine Benachrichtigung sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie mit der Überwachung voran, und aktivieren Sie sie jetzt.</span><span class="sxs-lookup"><span data-stu-id="f03fb-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f03fb-109">Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus vorherigen Datumsangaben ziehen.</span><span class="sxs-lookup"><span data-stu-id="f03fb-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f03fb-110">Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie in der Liste **Aktivitäten** aus. Andernfalls werden standardmäßig alle Aktivitäten für den ausgewählten Benutzer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f03fb-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="f03fb-111">Beachten Sie, dass bestimmte Aktivitäten möglicherweise nicht zur Auswahl im Menü **Aktivitäten verfügbar** sind. Diese Überwachungselemente werden jedoch zurückgegeben, wenn **Ergebnisse** für alle Aktivitäten anzeigen ausgewählt ist (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="f03fb-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="f03fb-112">Geben Sie den Datumsbereich an, und wählen Sie im Feld **Benutzer** den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten.</span><span class="sxs-lookup"><span data-stu-id="f03fb-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="f03fb-113">Wählen Sie **Suchen aus.**</span><span class="sxs-lookup"><span data-stu-id="f03fb-113">Select **Search**.</span></span> <span data-ttu-id="f03fb-114">Die Aktivitäten werden unter **Ergebnisse angezeigt.**</span><span class="sxs-lookup"><span data-stu-id="f03fb-114">The activities appear under **Results**.</span></span> <span data-ttu-id="f03fb-115">Sie können die IP-Adresse für jede Aktivität sehen.</span><span class="sxs-lookup"><span data-stu-id="f03fb-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="f03fb-116">Wählen Sie zum Anzeigen von Details eine Aktivität aus, und wählen Sie dann **Weitere Informationen aus.**</span><span class="sxs-lookup"><span data-stu-id="f03fb-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="f03fb-117">Weitere Informationen finden Sie unter Durchsuchen des [Office 365-Überwachungsprotokolls zur Problembehandlung gängiger Szenarien.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="f03fb-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>