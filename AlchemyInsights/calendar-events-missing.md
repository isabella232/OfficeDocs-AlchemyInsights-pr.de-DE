---
title: Kalenderereignisse fehlen oder werden nicht aktualisiert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819980"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="95918-102">Kalenderereignisse fehlen oder werden nicht aktualisiert</span><span class="sxs-lookup"><span data-stu-id="95918-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="95918-103">Wenn Kalenderelemente fehlen oder nicht aktualisiert werden, beginnen Sie mit der Überprüfung der Elementanzahl in den Eigenschaften Ihres Kalenderordners in Outlook:</span><span class="sxs-lookup"><span data-stu-id="95918-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="95918-104">Klicken Sie mit der rechten Maustaste auf den betroffenen Benutzer-**Kalenderordner** und dann auf **Eigenschaften**.</span><span class="sxs-lookup"><span data-stu-id="95918-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="95918-105">Wählen Sie die Registerkarte **Synchronisierung** aus.</span><span class="sxs-lookup"><span data-stu-id="95918-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="95918-106">Wenn die Elementanzahl im Serverordner nicht die gleiche wie die im Offlineordner ist:</span><span class="sxs-lookup"><span data-stu-id="95918-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="95918-107">Markieren Sie den **Kalenderordner**.</span><span class="sxs-lookup"><span data-stu-id="95918-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="95918-108">Wechseln Sie zur Registerkarte **Senden**/**Empfangen**, und klicken Sie dann auf **Ordner aktualisieren**.</span><span class="sxs-lookup"><span data-stu-id="95918-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="95918-109">Wenn Ihr Kalender immer noch nicht aktualisiert wird oder Ereignisse fehlen, laden Sie das Tool für die Kalenderüberprüfung für Outlook aus dem [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=28786) herunter.</span><span class="sxs-lookup"><span data-stu-id="95918-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="95918-110">Überprüfen Sie, ob der Kalenderordner mehr als 5.000 Elemente enthält, da dies zu Symptomen wie nicht aktualisierten Kalenderbesprechungen oder Besprechungsfehlern führen kann.</span><span class="sxs-lookup"><span data-stu-id="95918-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="95918-111">Weitere Informationen finden Sie unter [Outlook-Leistungsprobleme bei zu vielen Elementen oder Ordnern in einer OST- oder PST-Datei im Cachemodus](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span><span class="sxs-lookup"><span data-stu-id="95918-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>