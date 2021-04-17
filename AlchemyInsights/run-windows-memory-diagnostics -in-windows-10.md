---
title: Ausführen von Windows-Speicherdiagnose in Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826666"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="1536c-102">Ausführen von Windows-Speicherdiagnose in Windows 10</span><span class="sxs-lookup"><span data-stu-id="1536c-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="1536c-103">Wenn Windows und Apps auf Ihrem PC abstürzen, einfrieren oder sich instabil verhalten, haben Sie möglicherweise ein Problem mit dem Arbeitsspeicher (RAM) des PCs.</span><span class="sxs-lookup"><span data-stu-id="1536c-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="1536c-104">Sie können die Windows-Speicherdiagnose ausführen, um nach Problemen mit dem Arbeitsspeicher des PCs zu suchen.</span><span class="sxs-lookup"><span data-stu-id="1536c-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="1536c-105">Geben Sie in das Suchfeld in der Taskleiste **Speicherdiagnose** ein, und wählen Sie dann **Windows-Speicherdiagnose**.</span><span class="sxs-lookup"><span data-stu-id="1536c-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="1536c-106">Um die Diagnose auszuführen, muss der PC neu gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="1536c-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="1536c-107">Sie haben die Möglichkeit, sofort neu zu starten (bitte speichern Sie Ihre Arbeit und schließen Sie zuerst geöffnete Dokumente und E-Mails), oder Sie können die Diagnose so planen, dass sie beim nächsten Neustart des PCs automatisch ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="1536c-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows-Speicherdiagnose](media/windows-memory-diagnostic.png)

<span data-ttu-id="1536c-109">Wenn der PC neu gestartet wird, wird das **Windows-Speicherdiagnosetool** automatisch ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1536c-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="1536c-110">Status und Fortschritt werden während des Diagnoselaufs angezeigt, und Sie haben die Möglichkeit, die Diagnose durch Drücken der Taste **ESC** auf Ihrer Tastatur abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="1536c-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="1536c-111">Nach Abschluss der Diagnose wird Windows normal gestartet.</span><span class="sxs-lookup"><span data-stu-id="1536c-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="1536c-112">Unmittelbar nach dem Neustart, wenn der Desktop angezeigt wird, erscheint eine Benachrichtigung (neben dem Symbol  **Info-Center** in der Taskleiste), um anzuzeigen, ob Speicherfehler gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="1536c-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="1536c-113">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="1536c-113">For example:</span></span>

<span data-ttu-id="1536c-114">Das ist das Symbol „Info-Center“:</span><span class="sxs-lookup"><span data-stu-id="1536c-114">Here's the Action Center icon:</span></span> ![Symbol „Info-Center“](media/action-center-icon.png) 

<span data-ttu-id="1536c-116">Und eine Beispiel-Benachrichtigung:</span><span class="sxs-lookup"><span data-stu-id="1536c-116">And a sample notification:</span></span> ![Keine Speicherfehler](media/no-memory-errors.png)

<span data-ttu-id="1536c-118">Wenn Sie die Benachrichtigung verpasst haben, können Sie das Symbol **Info-Center** in der Taskleiste wählen, um das **Info-Center** anzuzeigen und eine scrollbare Liste der Benachrichtigungen zu sehen.</span><span class="sxs-lookup"><span data-stu-id="1536c-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="1536c-119">Um detaillierte Informationen zu überprüfen, geben Sie das **Ereignis** in das Suchfeld in Ihrer Taskleiste ein und wählen Sie dann **Ereignisanzeige**.</span><span class="sxs-lookup"><span data-stu-id="1536c-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="1536c-120">Navigieren Sie im linken Fensterbereich der **Ereignisanzeige** zu **Windows-Protokolle > System**.</span><span class="sxs-lookup"><span data-stu-id="1536c-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="1536c-121">Scannen Sie im rechten Fensterbereich die Liste nach unten, während Sie die Spalte **Quelle** betrachten, bis Sie Ereignisse mit dem Quellenwert **MemoryDiagnostics-Results** sehen.</span><span class="sxs-lookup"><span data-stu-id="1536c-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="1536c-122">Markieren Sie jedes dieser Ereignisse und sehen Sie die Ergebnisinformationen im Feld unter der Registerkarte **Allgemein** unterhalb der Liste.</span><span class="sxs-lookup"><span data-stu-id="1536c-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
