---
title: 'Fehler: die Regeln auf diesem Computer stimmen nicht überein'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617971"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="30594-102">Fehler: die Regeln auf diesem Computer stimmen nicht überein</span><span class="sxs-lookup"><span data-stu-id="30594-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="30594-103">Wenn Sie den aktualisierten Status dieses bekannten Problems sehen möchten, lesen Sie [die Regeln auf diesem Computer nicht mit den Regeln für Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="30594-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="30594-104">Das Outlook-Team hat ein Update in Build 12928,10000 implementiert.</span><span class="sxs-lookup"><span data-stu-id="30594-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="30594-105">Das Update ist bereits bei Insider fast und wird in den monatlichen Kanal Ende Juni 2020 gehen.</span><span class="sxs-lookup"><span data-stu-id="30594-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="30594-106">Sobald Sie den festen Build haben, erhalten Sie möglicherweise die Eingabeaufforderung "welche Regeln möchten Sie beibehalten?" ein letztes Mal.</span><span class="sxs-lookup"><span data-stu-id="30594-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="30594-107">Wählen Sie Server aus, wenn Sie dazu aufgefordert werden, und wechseln Sie dann in Outlook zurück, und aktivieren Sie alle deaktivierten Regeln erneut.</span><span class="sxs-lookup"><span data-stu-id="30594-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="30594-108">Verwenden Sie die folgende Problemumgehung, bis das Update verfügbar ist:</span><span class="sxs-lookup"><span data-stu-id="30594-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="30594-109">**Problemumgehung**: in den letzten Berichten ist das Problem bei denjenigen aufgetreten, die nur Clientregeln in Outlook-Desktop erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="30594-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="30594-110">Wenn Sie weiterhin auf das Problem stoßen, sollten Sie die Regeln löschen und dann Regeln nur in OWA (Outlook Web App) erstellen und bearbeiten, bis das Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="30594-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="30594-111">Wenn Sie die Regeln nicht manuell löschen können, können Sie beim Starten von Outlook einen Outlook-Befehl ausführen, indem Sie Outlook. exe/Cleanrules. ausführen.</span><span class="sxs-lookup"><span data-stu-id="30594-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="30594-112">Dadurch werden sowohl die Client-als auch die Server Regeln gelöscht.</span><span class="sxs-lookup"><span data-stu-id="30594-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="30594-113">Dadurch werden alle Regeln für alle Konten im Outlook-Profil gelöscht.</span><span class="sxs-lookup"><span data-stu-id="30594-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="30594-114">Dieser Befehl wird im Artikel Befehlszeilenoptionen weiter beschrieben.</span><span class="sxs-lookup"><span data-stu-id="30594-114">This command is further documented in the Command-line switches  article.</span></span>