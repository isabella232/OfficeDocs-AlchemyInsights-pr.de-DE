---
title: Problembehandlung bei Ereignissen aus E-Mails
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658733"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="d3a25-102">Problembehandlung bei Ereignissen aus E-Mails</span><span class="sxs-lookup"><span data-stu-id="d3a25-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="d3a25-103">Überprüfen Sie, ob das Feature für das Postfach aktiviert ist: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="d3a25-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="d3a25-104">Dann schauen Sie sich die "Ereignisse aus E-Mails"-Protokollen an: **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="d3a25-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="d3a25-105">Suchen Sie in den Protokollen "Ereignisse aus E-Mails" nach dem InternetMessageId, das dem Element im Postfach entspricht.</span><span class="sxs-lookup"><span data-stu-id="d3a25-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="d3a25-106">Die TrustScore bestimmt, ob das Element hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d3a25-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="d3a25-107">Ereignisse werden nur hinzugefügt, wenn die TrustScore = "vertrauenswürdig" lautet.</span><span class="sxs-lookup"><span data-stu-id="d3a25-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="d3a25-108">Die TrustScore wird durch die Eigenschaften SPF, Dkim oder Dmarc bestimmt, die sich im Nachrichtenkopf befinden.</span><span class="sxs-lookup"><span data-stu-id="d3a25-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="d3a25-109">So zeigen Sie diese Eigenschaften an:</span><span class="sxs-lookup"><span data-stu-id="d3a25-109">To view these properties:</span></span>

<span data-ttu-id="d3a25-110">**Desktop-Outlook**</span><span class="sxs-lookup"><span data-stu-id="d3a25-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="d3a25-111">Öffnen Sie das Element,</span><span class="sxs-lookup"><span data-stu-id="d3a25-111">Open the item</span></span>
- <span data-ttu-id="d3a25-112">Datei -> Eigenschaften -> Internet-Kopfzeilen</span><span class="sxs-lookup"><span data-stu-id="d3a25-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="d3a25-113">oder</span><span class="sxs-lookup"><span data-stu-id="d3a25-113">or</span></span>

<span data-ttu-id="d3a25-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="d3a25-114">**MFCMapi**</span></span>

- <span data-ttu-id="d3a25-115">Navigieren Sie zu dem Element im Posteingang</span><span class="sxs-lookup"><span data-stu-id="d3a25-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="d3a25-116">Suchen Sie nach PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="d3a25-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="d3a25-117">Diese Eigenschaften werden ermittelt und während des Transports und des Routings aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="d3a25-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="d3a25-118">Zur weiteren Problembehandlung müssen Sie möglicherweise die Transport Unterstützung zu den Fehlern in SPF, DKIM und/oder DMARC nachverfolgen.</span><span class="sxs-lookup"><span data-stu-id="d3a25-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>