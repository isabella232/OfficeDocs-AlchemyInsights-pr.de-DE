---
title: Problembehandlung bei Ereignissen aus E-Mails
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834838"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="c9f67-102">Problembehandlung bei Ereignissen aus E-Mails</span><span class="sxs-lookup"><span data-stu-id="c9f67-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="c9f67-103">Überprüfen Sie, ob das Feature für das Postfach aktiviert ist: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="c9f67-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="c9f67-104">Dann schauen Sie sich die "Ereignisse aus E-Mails"-Protokollen an: **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="c9f67-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="c9f67-105">Suchen Sie in den Protokollen "Ereignisse aus E-Mails" nach dem InternetMessageId, das dem Element im Postfach entspricht.</span><span class="sxs-lookup"><span data-stu-id="c9f67-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="c9f67-106">Die TrustScore bestimmt, ob das Element hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="c9f67-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="c9f67-107">Ereignisse werden nur hinzugefügt, wenn die TrustScore = "vertrauenswürdig" lautet.</span><span class="sxs-lookup"><span data-stu-id="c9f67-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="c9f67-108">Die TrustScore wird durch die Eigenschaften SPF, Dkim oder Dmarc bestimmt, die sich im Nachrichtenkopf befinden.</span><span class="sxs-lookup"><span data-stu-id="c9f67-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="c9f67-109">So zeigen Sie diese Eigenschaften an:</span><span class="sxs-lookup"><span data-stu-id="c9f67-109">To view these properties:</span></span>

<span data-ttu-id="c9f67-110">**Desktop-Outlook**</span><span class="sxs-lookup"><span data-stu-id="c9f67-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="c9f67-111">Öffnen Sie das Element,</span><span class="sxs-lookup"><span data-stu-id="c9f67-111">Open the item</span></span>
- <span data-ttu-id="c9f67-112">Datei -> Eigenschaften -> Internet-Kopfzeilen</span><span class="sxs-lookup"><span data-stu-id="c9f67-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="c9f67-113">oder</span><span class="sxs-lookup"><span data-stu-id="c9f67-113">or</span></span>

<span data-ttu-id="c9f67-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="c9f67-114">**MFCMapi**</span></span>

- <span data-ttu-id="c9f67-115">Navigieren Sie zu dem Element im Posteingang</span><span class="sxs-lookup"><span data-stu-id="c9f67-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="c9f67-116">Suchen Sie nach PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="c9f67-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="c9f67-117">Diese Eigenschaften werden ermittelt und während des Transports und des Routings aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="c9f67-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="c9f67-118">Zur weiteren Problembehandlung müssen Sie möglicherweise die Transport Unterstützung zu den Fehlern in SPF, DKIM und/oder DMARC nachverfolgen.</span><span class="sxs-lookup"><span data-stu-id="c9f67-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>