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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Ruhestand von vorversions-eDiscovery-Tools

Aufgrund der neuen und verbesserten eDiscovery-Funktionalität im Microsoft 365 Compliance Center werden die folgenden Legacy-eDiscovery-Tools und Cmdlets in den nächsten Monaten zurückgezogen:

- In [-Place-eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) und [in-Place-](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Speicher in der Exchange-Verwaltungskonsole.

- Die Exchange Online PowerShell-Cmdlets, die in-Place-eDiscovery und in-Place-Aufbewahrungen unterstützen. (Diese Cmdlets werden gemeinsam als *-MailboxSearch-Cmdlets identifiziert.) Dies umfasst die folgenden Cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Gruppe-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Das Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- Die folgenden Vorgänge in der Exchange Webdienste-API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Zeitachse für den Ruhestand**:
- 1. April 2020: Sie können keine neuen suchen und Aufbewahrungen erstellen, aber Sie können vorhandene Suchvorgänge auf eigenes Risiko ausführen, bearbeiten und löschen. Der Microsoft-Support unterstützt keine Compliance-eDiscovery-&, die in der Exchange-Verwaltungskonsole gespeichert sind.

- 1. Juli 2020: die in-situ-eDiscovery-&, in der die Exchange-Verwaltungskonsole Funktionen enthält, wird in den schreibgeschützten Modus versetzt. Dies bedeutet, dass Sie nur vorhandene suchen und Haltestatus entfernen können.

**Weitere Informationen finden Sie unter**:

 - [Migrieren von Legacy-eDiscovery-suchen und-Archiven zum Microsoft 365 Compliance Center](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Ruhestand von vorversions-eDiscovery-Tools](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQs zu Compliance-eDiscovery und in-Place-Archiven](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



