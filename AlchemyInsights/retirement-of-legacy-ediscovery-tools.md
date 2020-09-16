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

- [Erweiterte eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Zeitachse für den Ruhestand**:
- **1. Juli 2020** Sie können keine neuen suchen und Aufbewahrungen mehr erstellen, aber Sie können vorhandene Suchvorgänge auf eigenes Risiko ausführen, bearbeiten und löschen. Der Microsoft-Support unterstützt keine Compliance-eDiscovery-& mehr in der Exchange-Verwaltungskonsole.
    
- **1. Oktober 2020** In-situ-eDiscovery-& die Funktionen in der Exchange-Verwaltungskonsole enthalten, werden in den schreibgeschützten Modus versetzt, sodass Sie nur vorhandene suchen und Haltestatus entfernen können.

**Weitere Informationen finden Sie unter**:

 - [Migrieren von Legacy-eDiscovery-suchen und-Archiven zum Microsoft 365 Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Einstellung älterer eDiscovery-Tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQs zu Compliance-eDiscovery und in-Place-Archiven](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



