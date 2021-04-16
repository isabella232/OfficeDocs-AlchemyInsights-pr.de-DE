---
title: Error-AttributValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813759"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributValueMustBeUnique

Der häufigste Grund für den AttributValueMustBeUnique-Fehler ist, dass zwei Objekte mit unterschiedlichen SourceAnchor (immutableId) denselben Wert für die Attribute ProxyAddresses und/oder UserPrincipalName aufweisen. So beheben Sie den AttributValueMustBeUnique-Fehler:
  
1. Identifizieren Sie die duplizierten proxyAddresses, userPrincipalName oder einen anderen Attributwert, der den Fehler verursacht. Identifizieren Sie außerdem, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der von Azure AD Connect Health für die Synchronisierung generierte Bericht kann Ihnen dabei helfen, die beiden Objekte zu identifizieren.
    
2. Identifizieren Sie, welches Objekt weiterhin den duplizierten Wert haben soll und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das DIESEN Wert NICHT haben sollte. Beachten Sie, dass Sie die Änderung im Verzeichnis, aus dem das Objekt stammt, ändern sollten. In einigen Fällen müssen Sie möglicherweise eines der objekte löschen, die in Konflikt stehen.
    
4. Wenn Sie die Änderung im lokalen AD vorgenommen haben, lassen Sie Azure AD Connect die Änderung synchronisieren, damit der Fehler behoben wird.
    

