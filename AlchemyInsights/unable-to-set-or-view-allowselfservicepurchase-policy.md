---
title: Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden.
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826090"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden.

Wenn Sie versuchen, die AllowSelfServicePurchase-Richtlinie zu festlegen oder anzeigen, wird die folgende Fehlermeldung angezeigt:

*HandleError : Fehler beim Abrufen der Produktrichtlinie mit PolicyId 'AllowSelfServicePurchase', ErrorMessage – Die zugrunde liegende Verbindung wurde geschlossen: Bei einem Senden ist ein unerwarteter Fehler aufgetreten.*

Dies liegt möglicherweise an einer älteren Version von Transport Layer Security (TLS). Zum Verbinden des MS Commerce-Diensts müssen Sie TLS 1.2 oder höher verwenden.  

Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1.2 zu aktivieren bzw. auf 1.2 zu setzen, zu überprüfen und erneut zu versuchen.
 1. Geben Sie an der #A0 (PS C: geben Sie den folgenden Befehl ein, um das \) #A1 auf Version 1.2 zu setzen:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Überprüfen Sie die verwendeten TLS-Protokolle mit dem folgenden Befehl:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Wiederholen Sie die Befehle Get oder Update nach Bedarf.

