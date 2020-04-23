---
title: SharePoint-umfangreiche Listen
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767284"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="a26fe-102">Arbeiten mit umfangreichen Listen und Bibliotheken in SharePoint</span><span class="sxs-lookup"><span data-stu-id="a26fe-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="a26fe-103">SharePoint-Listen und-Bibliotheken können bis zu 30 Millionen Elemente enthalten, wenn Sie jedoch über mehr als 5.000 Elemente verfügen, wird möglicherweise ein Schwellenwert für die Listenansicht angezeigt, wenn Sie versuchen, mit Ihnen zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="a26fe-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="a26fe-104">Dieser Schwellenwert dient dazu, die Leistung des Diensts aufrechtzuerhalten.</span><span class="sxs-lookup"><span data-stu-id="a26fe-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="a26fe-105">Er kann nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="a26fe-105">It can't be changed.</span></span> <span data-ttu-id="a26fe-106">Um zu vermeiden, dass dieser Schwellenwert erreicht wird:</span><span class="sxs-lookup"><span data-stu-id="a26fe-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="a26fe-107">**Moderne Nutzung**</span><span class="sxs-lookup"><span data-stu-id="a26fe-107">**Use modern**</span></span>

<span data-ttu-id="a26fe-108">Ansichten mit vielen Elementen funktionieren am besten in der modernen Benutzeroberfläche.</span><span class="sxs-lookup"><span data-stu-id="a26fe-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="a26fe-109">[Verwenden Sie die moderne Benutzeroberfläche](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , um Fehler zu vermeiden, die möglicherweise in der klassischen Umgebung angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a26fe-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="a26fe-110">**Hinzufügen von Indizes**</span><span class="sxs-lookup"><span data-stu-id="a26fe-110">**Add indexes**</span></span>

<span data-ttu-id="a26fe-111">Wenn Sie nach einer Spalte filtern oder sortieren, die keinen Index aufweist, wird möglicherweise eine Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a26fe-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="a26fe-112">Manuelles [Hinzufügen eines Index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) aus den **Listeneinstellungen** im Menü "Einstellungen" und dann aus **indizierten Spalten**.</span><span class="sxs-lookup"><span data-stu-id="a26fe-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="a26fe-113">**Bearbeiten der Listenansicht**</span><span class="sxs-lookup"><span data-stu-id="a26fe-113">**Edit the list view**</span></span>

<span data-ttu-id="a26fe-114">Wenn beim Arbeiten mit einer umfangreichen Liste ein Fehler auftritt, [Bearbeiten Sie die Listenansicht](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="a26fe-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="a26fe-115">Mit den folgenden vier Änderungen werden Schwellenwert Fehler in der Listenansicht entfernt.</span><span class="sxs-lookup"><span data-stu-id="a26fe-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="a26fe-116">Nehmen Sie alle vier Änderungen vor, um alle Fehler zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="a26fe-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="a26fe-117">Wenn Sie weiterhin Fehler erhalten, überprüfen Sie die [Verwaltung umfangreicher Listen und Bibliotheken](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="a26fe-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="a26fe-118">Wählen Sie **None** aus, **indem Sie zuerst nach der Spalte sortieren** und **dann nach der Spalte sortieren**.</span><span class="sxs-lookup"><span data-stu-id="a26fe-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="a26fe-119">Wählen Sie **None** aus **der ersten Gruppe nach der Spalte** aus, und **Gruppieren Sie dann nach der Spalte**.</span><span class="sxs-lookup"><span data-stu-id="a26fe-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="a26fe-120">Wählen Sie **None** für alle Spalten im Abschnitt **Summen** aus.</span><span class="sxs-lookup"><span data-stu-id="a26fe-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="a26fe-121">Deaktivieren Sie im Abschnitt **Spalten** die Option Alle bis auf eine Spalte für die Anzeige.</span><span class="sxs-lookup"><span data-stu-id="a26fe-121">Deselect all but one column for display from the **Columns** section.</span></span>

