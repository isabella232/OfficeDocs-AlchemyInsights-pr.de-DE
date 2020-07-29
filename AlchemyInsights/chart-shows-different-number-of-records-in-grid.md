---
title: Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431632"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="06dcf-102">Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster</span><span class="sxs-lookup"><span data-stu-id="06dcf-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="06dcf-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="06dcf-103">**Symptom**</span></span>

<span data-ttu-id="06dcf-104">Wenn Sie bei einem Diagramm auf der Dashboardseite auf das Diagramm „...“ klicken und auf „Datensätze anzeigen“ klicken, navigieren Sie zur Rasterseite, um alle Datensätze zu sehen. Manchmal ändert sich die Anzahl der Datensätze.</span><span class="sxs-lookup"><span data-stu-id="06dcf-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="06dcf-105">**Ursache**</span><span class="sxs-lookup"><span data-stu-id="06dcf-105">**Cause**</span></span>

<span data-ttu-id="06dcf-106">Dies ist auf die unterschiedlichen Ansichten zwischen dem Diagramm auf der ursprünglichen Dashboardseite und dem Diagramm auf der Rasterstartseite zurückzuführen.</span><span class="sxs-lookup"><span data-stu-id="06dcf-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="06dcf-107">**Lösung**</span><span class="sxs-lookup"><span data-stu-id="06dcf-107">**Solution**</span></span>

1. <span data-ttu-id="06dcf-108">Überprüfen Sie die Ansicht auf der ursprünglichen Seite und der Ansicht im Raster, um zu sehen, ob Sie anders sind.</span><span class="sxs-lookup"><span data-stu-id="06dcf-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="06dcf-109">Ändern Sie die Ansicht im Raster so, dass sie der Ansicht auf der ursprünglichen Seite entspricht.</span><span class="sxs-lookup"><span data-stu-id="06dcf-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="06dcf-110">Wenn die richtige Darstellung nicht gefunden werden kann, bedeutet dies normalerweise, dass die Ansicht im App-Designer nicht aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="06dcf-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="06dcf-111">Wechseln Sie zum App-Designer der jeweiligen App, wählen Sie die Entität und deren Ansichten aus, überprüfen Sie die Ansicht, die Sie aktivieren, speichern, veröffentlichen und schließen möchten.</span><span class="sxs-lookup"><span data-stu-id="06dcf-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="06dcf-112">Aktualisieren Sie die Seite.</span><span class="sxs-lookup"><span data-stu-id="06dcf-112">Refresh the page.</span></span>