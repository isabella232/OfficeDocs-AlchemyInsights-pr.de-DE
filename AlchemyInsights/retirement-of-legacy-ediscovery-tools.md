---
title: Rente von Legacy-eDiscovery-Tools
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798548"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="9eecd-102">Rente von Legacy-eDiscovery-Tools</span><span class="sxs-lookup"><span data-stu-id="9eecd-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="9eecd-103">Aufgrund der neuen und verbesserten eDiscovery-Funktionalität im Microsoft 365 Compliance Center werden die folgenden älteren eDiscovery-Tools und -Befehlslets in den kommenden Monaten eingestellt:</span><span class="sxs-lookup"><span data-stu-id="9eecd-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="9eecd-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) und [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) im Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="9eecd-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="9eecd-105">Die Exchange Online PowerShell-Cmdlets, die In-Place eDiscovery und In-Place unterstützen.</span><span class="sxs-lookup"><span data-stu-id="9eecd-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="9eecd-106">(Diese Cmdlets werden gemeinsam als \*-MailboxSearch-Cmdlets identifiziert.) Dies umfasst die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9eecd-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="9eecd-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9eecd-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="9eecd-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9eecd-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="9eecd-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9eecd-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="9eecd-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9eecd-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="9eecd-111">Das [Cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9eecd-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="9eecd-112">Die folgenden Vorgänge in der Exchange Web Services-API:</span><span class="sxs-lookup"><span data-stu-id="9eecd-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="9eecd-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9eecd-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="9eecd-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9eecd-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="9eecd-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9eecd-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="9eecd-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="9eecd-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="9eecd-117">**Zeitachse für die Rente**:</span><span class="sxs-lookup"><span data-stu-id="9eecd-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="9eecd-118">**1. Juli 2020** Sie können keine neuen Such- und Haltekriterien mehr erstellen, aber Sie können vorhandene Suchen auf eigenes Risiko ausführen, bearbeiten und löschen.</span><span class="sxs-lookup"><span data-stu-id="9eecd-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="9eecd-119">Der Microsoft Support unterstützt In-Place eDiscovery & in der EAC nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="9eecd-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="9eecd-120">**1. Oktober 2020** In-Place eDiscovery & Die Funktionen "Holds" in der EAC werden im schreibgeschützten Modus platziert, sodass Sie nur vorhandene Such- und Haltefunktionen entfernen können.</span><span class="sxs-lookup"><span data-stu-id="9eecd-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="9eecd-121">**Weitere Informationen finden Sie unter**:</span><span class="sxs-lookup"><span data-stu-id="9eecd-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="9eecd-122">Migrieren von älteren eDiscovery-Suchen und -Haltedaten zum Microsoft 365 Compliance Center</span><span class="sxs-lookup"><span data-stu-id="9eecd-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="9eecd-123">Einstellung älterer eDiscovery-Tools</span><span class="sxs-lookup"><span data-stu-id="9eecd-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="9eecd-124">Häufig gestellte Fragen In-Place eDiscovery und In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="9eecd-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



