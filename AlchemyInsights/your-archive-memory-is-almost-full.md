---
title: Ihr Archivpostfach ist fast voll
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950508"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Ihr Archivpostfach ist fast voll

Wenn der Benutzer die Warnung erhält; **Ihr Archivpostfach ist fast voll,** oder Sie müssen die Größe ihres Archivpostfachs erhöhen. Hier sind einige Tipps:

1. Wenn dem Benutzer ein Exchange Online Plan 1 zugewiesen ist, aktualisieren Sie auf **die Exchange Online Plan 2-Lizenz,** um die Größe von 50 GB auf 100 GB zu erhöhen.
1. Wenn dem Benutzer bereits einer der folgenden Optionen zugewiesen ist: **Exchange Online Plan 2** oder Exchange Online Plan 1 mit einem Exchange Online-Archivierung-Add-On, verwenden Sie die folgenden Schritte, um die Archivierung mit automatischer Erweiterung zu aktivieren:
 
    1. [Stellen Sie eine Verbindung mit Exchange Online Powershell herstellen.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Führen Sie das folgende Befehlslet für den Benutzer aus:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Führen Sie das folgende Befehlslet aus, um zu bestätigen, dass es für den Benutzer aktiviert ist:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Weitere Informationen finden Sie unter:

- [ Unbegrenzte Archivierung aktivieren – Administratorhilfe – Microsoft 365 Compliance | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online-Beschränkungen – Dienstbeschreibungen | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade auf einen anderen Geschäftsplan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

