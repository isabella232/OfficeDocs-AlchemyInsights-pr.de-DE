---
title: 'Fehler: Die Regeln auf diesem Computer entsprechen nicht'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782951"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="40c52-102">Fehler: Die Regeln auf diesem Computer entsprechen nicht</span><span class="sxs-lookup"><span data-stu-id="40c52-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="40c52-103">Informationen zum aktualisierten Status dieses bekannten Problems finden Sie unter Die Regeln auf diesem Computer entsprechen nicht den [Regeln in Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="40c52-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="40c52-104">Das Outlook-Team hat eine Korrektur in Build 12928.10000 implementiert.</span><span class="sxs-lookup"><span data-stu-id="40c52-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="40c52-105">Der Fix ist bereits bei Insider Fast und wird Ende Juni 2020 zum monatlichen Kanal wechseln.</span><span class="sxs-lookup"><span data-stu-id="40c52-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="40c52-106">Sobald Sie den festen Build haben, erhalten Sie möglicherweise ein letztes Mal die Eingabeaufforderung "Welche Regeln möchten Sie behalten".</span><span class="sxs-lookup"><span data-stu-id="40c52-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="40c52-107">Wählen Sie Server, wenn Sie dazu aufgefordert werden, und wechseln Sie dann zurück in Outlook, und aktivieren Sie alle deaktivierten Regeln erneut.</span><span class="sxs-lookup"><span data-stu-id="40c52-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="40c52-108">Verwenden Sie die folgende Problemumgehung, bis die Korrektur verfügbar ist:</span><span class="sxs-lookup"><span data-stu-id="40c52-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="40c52-109">**Problemumgehung**: In den letzten Berichten ist das Problem für diejenigen aufgetreten, die nur Clientregeln in Outlook Desktop erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="40c52-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="40c52-110">Wenn das Problem weiterhin besteht, sollten Sie die Regeln löschen und regeln dann nur in OWA (Outlook Web App) erstellen und bearbeiten, bis das Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="40c52-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="40c52-111">Wenn Sie die Regeln nicht manuell löschen können, können Sie beim Starten von Outlook einen Outlook-Befehl ausführen, indem Sie Outlook.exe /cleanrules ausführen.</span><span class="sxs-lookup"><span data-stu-id="40c52-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="40c52-112">Dadurch werden sowohl die Client- als auch die Serverregeln gelöscht.</span><span class="sxs-lookup"><span data-stu-id="40c52-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="40c52-113">Es werden alle Regeln für alle Konten im Outlook-Profil gelöscht.</span><span class="sxs-lookup"><span data-stu-id="40c52-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="40c52-114">Dieser Befehl wird im Artikel Befehlszeilenschalter weiter dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="40c52-114">This command is further documented in the Command-line switches article.</span></span>

