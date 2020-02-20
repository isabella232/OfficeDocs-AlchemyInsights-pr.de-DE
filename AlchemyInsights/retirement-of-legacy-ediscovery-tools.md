---
title: Ruhestand von vorversions-eDiscovery-Tools
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157588"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="bb2da-102">Ruhestand von vorversions-eDiscovery-Tools</span><span class="sxs-lookup"><span data-stu-id="bb2da-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="bb2da-103">Aufgrund der neuen und verbesserten eDiscovery-Funktionalität im Microsoft 365 Compliance Center werden die folgenden Legacy-eDiscovery-Tools und Cmdlets in den nächsten Monaten zurückgezogen:</span><span class="sxs-lookup"><span data-stu-id="bb2da-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="bb2da-104">In [-Place-eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) und [in-Place-](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Speicher in der Exchange-Verwaltungskonsole.</span><span class="sxs-lookup"><span data-stu-id="bb2da-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="bb2da-105">Die Exchange Online PowerShell-Cmdlets, die in-Place-eDiscovery und in-Place-Aufbewahrungen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="bb2da-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="bb2da-106">(Diese Cmdlets werden gemeinsam als \*-MailboxSearch-Cmdlets identifiziert.) Dies umfasst die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="bb2da-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="bb2da-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bb2da-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="bb2da-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bb2da-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="bb2da-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bb2da-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="bb2da-110">Gruppe-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bb2da-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="bb2da-111">Das Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bb2da-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="bb2da-112">Die folgenden Vorgänge in der Exchange Webdienste-API:</span><span class="sxs-lookup"><span data-stu-id="bb2da-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="bb2da-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="bb2da-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="bb2da-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bb2da-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="bb2da-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bb2da-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="bb2da-116">Office 365 Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="bb2da-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="bb2da-117">**Zeitachse für den Ruhestand**:</span><span class="sxs-lookup"><span data-stu-id="bb2da-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="bb2da-118">1. April 2020: Sie können keine neuen suchen und Aufbewahrungen erstellen, aber Sie können vorhandene Suchvorgänge auf eigenes Risiko ausführen, bearbeiten und löschen.</span><span class="sxs-lookup"><span data-stu-id="bb2da-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="bb2da-119">Der Microsoft-Support unterstützt keine Compliance-eDiscovery-&, die in der Exchange-Verwaltungskonsole gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="bb2da-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="bb2da-120">1. Juli 2020: die in-situ-eDiscovery-&, in der die Exchange-Verwaltungskonsole Funktionen enthält, wird in den schreibgeschützten Modus versetzt.</span><span class="sxs-lookup"><span data-stu-id="bb2da-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="bb2da-121">Dies bedeutet, dass Sie nur vorhandene suchen und Haltestatus entfernen können.</span><span class="sxs-lookup"><span data-stu-id="bb2da-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="bb2da-122">**Weitere Informationen finden Sie unter**:</span><span class="sxs-lookup"><span data-stu-id="bb2da-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="bb2da-123">Migrieren von Legacy-eDiscovery-suchen und-Archiven zum Microsoft 365 Compliance Center</span><span class="sxs-lookup"><span data-stu-id="bb2da-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="bb2da-124">Ruhestand von vorversions-eDiscovery-Tools</span><span class="sxs-lookup"><span data-stu-id="bb2da-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="bb2da-125">FAQs zu Compliance-eDiscovery und in-Place-Archiven</span><span class="sxs-lookup"><span data-stu-id="bb2da-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



