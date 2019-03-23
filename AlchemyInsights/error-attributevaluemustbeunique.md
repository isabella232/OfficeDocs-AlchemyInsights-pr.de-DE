---
title: Fehler AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766023"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler ist zwei Objekte mit verschiedenen Attributs (unveränderlichen) haben den gleichen Wert für die Attribute ProxyAddresses und/oder UserPrincipalName. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie den duplizierten proxyAddresses, userPrincipalName oder anderen Attributwert, der den Fehler verursacht. Identifizieren Sie auch, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der von Azure AD Connect Health for Sync generierte Bericht hilft Ihnen bei der Identifizierung der beiden Objekte.
    
2. Bestimmen Sie, welches Objekt weiterhin den doppelten Wert aufweisen sollte und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, der diesen Wert nicht aufweisen sollte. Beachten Sie, dass Sie die Änderung im Verzeichnis vornehmen sollten, aus dem das Objekt stammt. In einigen Fällen müssen Sie möglicherweise eines der Objekte in Konflikt löschen.
    
4. Wenn Sie die Änderung in der lokalen AD vorgenommen haben, lassen Sie Azure AD Connect die Änderung synchronisieren, damit der Fehler behoben wird.
    

