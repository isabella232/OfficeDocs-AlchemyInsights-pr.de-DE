---
title: Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091702"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden

Beim Versuch, die AllowSelfServicePurchase-Richtlinie festzulegen oder anzuzeigen, wird die folgende Fehlermeldung angezeigt:

*HandleError: Fehler beim Abrufen der Produktrichtlinie mit der Richtlinien-Nr "AllowSelfServicePurchase", ErrorMessage – die zugrunde liegende Verbindung wurde geschlossen: ein unerwarteter Fehler ist bei einem senden aufgetreten.*

Dies kann an einer älteren Version von Transport Layer Security (TLS) liegen. Um den MSCommerce-Dienst zu verbinden, müssen Sie TLS 1,2 oder höher verwenden.  

Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1,2, überprüfen und wiederholen zu aktivieren/festzulegen.
 1. Geben Sie an der PowerShell-Eingabeaufforderung (\) PS C: den folgenden Befehl ein, um das TLS-Protokoll auf Version 1,2 festzulegen:

    \[NET. ServicePointManager]:: SecurityProtocol \[= net. SecurityProtocolType]:: Tls12

2. Überprüfen Sie mit dem folgenden Befehl die verwendeten TLS-Protokolle (n):

    \[NET. ServicePointManager]:: SecurityProtocol 

3. Wiederholen Sie die Befehle Get oder Update bei Bedarf.

