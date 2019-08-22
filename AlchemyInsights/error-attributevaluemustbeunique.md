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
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526991"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler ist, dass zwei Objekte mit unterschiedlichen Attributs (unveränderlich) denselben Wert für die Attribute proxyAddresses und/oder userPrincipalName haben. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie den doppelten proxyAddresses-, userPrincipalName-oder other-Attributwert, der den Fehler verursacht. Ermitteln Sie auch, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der Bericht, der von Azure AD Connect-Integrität für Sync generiert wird, kann Ihnen dabei helfen, die beiden Objekte zu identifizieren.
    
2. Ermitteln Sie, welches Objekt weiterhin den doppelten Wert aufweisen soll und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das diesen Wert nicht aufweisen sollte. Beachten Sie, dass Sie die Änderung in dem Verzeichnis vornehmen sollten, aus dem das objektbezogen wird. In einigen Fällen müssen Sie möglicherweise eines der in Konflikt stehenden Objekte löschen.
    
4. Wenn Sie die Änderung in der lokalen AD vorgenommen haben, lassen Sie Azure AD Connect Sync die Änderung für den Fehler behoben erhalten.
    

