---
title: Fehler AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703173"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler ist, dass zwei Objekte mit unterschiedlichen Attributs (unveränderlich) denselben Wert für die Attribute proxyAddresses und/oder userPrincipalName haben. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie den doppelten proxyAddresses-, userPrincipalName-oder other-Attributwert, der den Fehler verursacht. Ermitteln Sie auch, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der Bericht, der von Azure AD Connect-Integrität für Sync generiert wird, kann Ihnen dabei helfen, die beiden Objekte zu identifizieren.
    
2. Ermitteln Sie, welches Objekt weiterhin den doppelten Wert aufweisen soll und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das diesen Wert nicht aufweisen sollte. Beachten Sie, dass Sie die Änderung in dem Verzeichnis vornehmen sollten, aus dem das objektbezogen wird. In einigen Fällen müssen Sie möglicherweise eines der in Konflikt stehenden Objekte löschen.
    
4. Wenn Sie die Änderung in der lokalen AD vorgenommen haben, lassen Sie Azure AD Connect Sync die Änderung für den Fehler behoben erhalten.
    

