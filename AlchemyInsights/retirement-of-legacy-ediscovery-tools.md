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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Rente von Legacy-eDiscovery-Tools

Aufgrund der neuen und verbesserten eDiscovery-Funktionalität im Microsoft 365 Compliance Center werden die folgenden älteren eDiscovery-Tools und -Befehlslets in den kommenden Monaten eingestellt:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) und [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) im Exchange Admin Center.

- Die Exchange Online PowerShell-Cmdlets, die In-Place eDiscovery und In-Place unterstützen. (Diese Cmdlets werden gemeinsam als *-MailboxSearch-Cmdlets identifiziert.) Dies umfasst die folgenden Cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Das [Cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- Die folgenden Vorgänge in der Exchange Web Services-API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Zeitachse für die Rente**:
- **1. Juli 2020** Sie können keine neuen Such- und Haltekriterien mehr erstellen, aber Sie können vorhandene Suchen auf eigenes Risiko ausführen, bearbeiten und löschen. Der Microsoft Support unterstützt In-Place eDiscovery & in der EAC nicht mehr.
    
- **1. Oktober 2020** In-Place eDiscovery & Die Funktionen "Holds" in der EAC werden im schreibgeschützten Modus platziert, sodass Sie nur vorhandene Such- und Haltefunktionen entfernen können.

**Weitere Informationen finden Sie unter**:

 - [Migrieren von älteren eDiscovery-Suchen und -Haltedaten zum Microsoft 365 Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Einstellung älterer eDiscovery-Tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Häufig gestellte Fragen In-Place eDiscovery und In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



