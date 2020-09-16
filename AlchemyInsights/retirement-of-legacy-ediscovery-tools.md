---
title: Ruhestand von vorversions-eDiscovery-Tools
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727782"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="7b940-102">Ruhestand von vorversions-eDiscovery-Tools</span><span class="sxs-lookup"><span data-stu-id="7b940-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="7b940-103">Aufgrund der neuen und verbesserten eDiscovery-Funktionalität im Microsoft 365 Compliance Center werden die folgenden Legacy-eDiscovery-Tools und Cmdlets in den nächsten Monaten zurückgezogen:</span><span class="sxs-lookup"><span data-stu-id="7b940-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="7b940-104">In [-Place-eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) und [in-Place-](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Speicher in der Exchange-Verwaltungskonsole.</span><span class="sxs-lookup"><span data-stu-id="7b940-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="7b940-105">Die Exchange Online PowerShell-Cmdlets, die in-Place-eDiscovery und in-Place-Aufbewahrungen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="7b940-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="7b940-106">(Diese Cmdlets werden gemeinsam als \*-MailboxSearch-Cmdlets identifiziert.) Dies umfasst die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7b940-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="7b940-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7b940-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="7b940-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7b940-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="7b940-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7b940-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="7b940-110">Gruppe-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7b940-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="7b940-111">Das Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7b940-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="7b940-112">Die folgenden Vorgänge in der Exchange Webdienste-API:</span><span class="sxs-lookup"><span data-stu-id="7b940-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="7b940-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7b940-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="7b940-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7b940-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="7b940-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7b940-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="7b940-116">Erweiterte eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="7b940-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="7b940-117">**Zeitachse für den Ruhestand**:</span><span class="sxs-lookup"><span data-stu-id="7b940-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="7b940-118">**1. Juli 2020** Sie können keine neuen suchen und Aufbewahrungen mehr erstellen, aber Sie können vorhandene Suchvorgänge auf eigenes Risiko ausführen, bearbeiten und löschen.</span><span class="sxs-lookup"><span data-stu-id="7b940-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="7b940-119">Der Microsoft-Support unterstützt keine Compliance-eDiscovery-& mehr in der Exchange-Verwaltungskonsole.</span><span class="sxs-lookup"><span data-stu-id="7b940-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="7b940-120">**1. Oktober 2020** In-situ-eDiscovery-& die Funktionen in der Exchange-Verwaltungskonsole enthalten, werden in den schreibgeschützten Modus versetzt, sodass Sie nur vorhandene suchen und Haltestatus entfernen können.</span><span class="sxs-lookup"><span data-stu-id="7b940-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="7b940-121">**Weitere Informationen finden Sie unter**:</span><span class="sxs-lookup"><span data-stu-id="7b940-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="7b940-122">Migrieren von Legacy-eDiscovery-suchen und-Archiven zum Microsoft 365 Compliance Center</span><span class="sxs-lookup"><span data-stu-id="7b940-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="7b940-123">Einstellung älterer eDiscovery-Tools</span><span class="sxs-lookup"><span data-stu-id="7b940-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="7b940-124">FAQs zu Compliance-eDiscovery und in-Place-Archiven</span><span class="sxs-lookup"><span data-stu-id="7b940-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



