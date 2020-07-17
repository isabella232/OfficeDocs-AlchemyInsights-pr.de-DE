---
title: Druckerspoolerproblem wurde behoben
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083949"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="4d01b-102">Druckerspoolerproblem wurde behoben</span><span class="sxs-lookup"><span data-stu-id="4d01b-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="4d01b-103">Wenn Ihr Gerät mit Windows 10 **OS Build 19041.329** aktualisiert wurde, kann es bei bestimmten Druckern zu einem Problem gekommen sein.</span><span class="sxs-lookup"><span data-stu-id="4d01b-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="4d01b-104">Der Druckerspooler löste beim Versuch zu drucken möglicherweise einen Fehler aus oder wurde unerwartet beendet, und es wurde vom betroffenen Drucker keine Ausgabe gedruckt.</span><span class="sxs-lookup"><span data-stu-id="4d01b-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="4d01b-105">Dieses Problem wurde in Betriebssystembuild **19041.331** behoben ([KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)).</span><span class="sxs-lookup"><span data-stu-id="4d01b-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="4d01b-106">**Untersuchung läuft**</span><span class="sxs-lookup"><span data-stu-id="4d01b-106">**Ongoing investigation**</span></span>

<span data-ttu-id="4d01b-107">Die LSASS-Datei (Local Security Authority Subsystem Service), **Isass.exe**, schlägt auf einigen Geräten mit der Fehlermeldung "Fehler bei einem kritischen Systemprozess, C:\WINDOWS\system32\Isass.exe, mit Statuscode c0000008.</span><span class="sxs-lookup"><span data-stu-id="4d01b-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="4d01b-108">Der Computer muss jetzt neu gestartet werden" fehl.</span><span class="sxs-lookup"><span data-stu-id="4d01b-108">The machine must now be restarted".</span></span>  <span data-ttu-id="4d01b-109">**Microsoft arbeitet an einer Lösung und stellt in einer kommenden Version ein Update bereit.**</span><span class="sxs-lookup"><span data-stu-id="4d01b-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="4d01b-110">Weitere Informationen finden Sie unter [Bekannte Probleme in Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="4d01b-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>