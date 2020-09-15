---
title: Fehler AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709150"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler ist, dass zwei Objekte mit unterschiedlichen Attributs (unveränderlich) denselben Wert für die Attribute proxyAddresses und/oder userPrincipalName haben. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie den doppelten proxyAddresses-, userPrincipalName-oder other-Attributwert, der den Fehler verursacht. Ermitteln Sie auch, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der Bericht, der von Azure AD Connect-Integrität für Sync generiert wird, kann Ihnen dabei helfen, die beiden Objekte zu identifizieren.
    
2. Ermitteln Sie, welches Objekt weiterhin den doppelten Wert aufweisen soll und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das diesen Wert nicht aufweisen sollte. Beachten Sie, dass Sie die Änderung in dem Verzeichnis vornehmen sollten, aus dem das objektbezogen wird. In einigen Fällen müssen Sie möglicherweise eines der in Konflikt stehenden Objekte löschen.
    
4. Wenn Sie die Änderung in der lokalen AD vorgenommen haben, lassen Sie Azure AD Connect Sync die Änderung für den Fehler behoben erhalten.
    

