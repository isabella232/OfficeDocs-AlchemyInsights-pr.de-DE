---
title: Fix user policy/mailbox settings
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568570"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="29cee-102">Fix user policy/mailbox settings</span><span class="sxs-lookup"><span data-stu-id="29cee-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="29cee-103">Die Junk-E-Mail-Einstellungen für das Postfach haben diese Nachricht beeinflusst.</span><span class="sxs-lookup"><span data-stu-id="29cee-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="29cee-104">Gehen Sie wie folgt vor, um die Einstellungen zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="29cee-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="29cee-105">Starten Sie die Exchange-Verwaltungsshell.</span><span class="sxs-lookup"><span data-stu-id="29cee-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="29cee-106">Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="29cee-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="29cee-107">Führen Sie diesen Befehl aus (unter Verwendung der  **E-Mail-Adresse des Benutzers): get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="29cee-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="29cee-108">Überprüfen Sie, ob die E-Mail-Adresse des Absenders Teil von **TrustedSendersAndDomains** oder **BlockedSendersAndDomains ist.**</span><span class="sxs-lookup"><span data-stu-id="29cee-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="29cee-109">Wenn sich die E-Mail-Adresse in einer der Listen befindet, müssen Sie sie möglicherweise entfernen.</span><span class="sxs-lookup"><span data-stu-id="29cee-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="29cee-110">Weitere Informationen finden Sie unter [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="29cee-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
