---
title: Fehler AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289695"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Die häufigste Ursache für den Fehler AttributeValueMustBeUnique ist, dass zwei Objekte mit unterschiedlichen SourceAnchor (ImmutableId) den gleichen Wert für die ProxyAddresses und/oder UserPrincipalName-Attribute aufweisen. Zu den AttributeValueMustBeUnique Fehler zu beheben:
  
1. Identifizieren Sie die duplizierte ProxyAddresses, UserPrincipalName oder anderen Attributwert, der den Fehler verursacht. Auch bestimmen Sie, welche Objekte (mindestens zwei) an den Konflikt beteiligt sind. Der Bericht von Azure Active Directory verbinden Integrität bei der Synchronisierung generierte helfen Ihnen die zwei Objekte identifizieren.
    
2. Ermitteln Sie, welches Objekt duplizierten Wert haben fortgesetzt werden soll und welche Objekt sollte nicht.
    
3. Entfernen des duplizierten Werts aus dem Objekt, das nicht den Wert verfügen soll. Beachten Sie, dass Sie die Änderung in das Verzeichnis, in dem das Objekt aus stammende ist, machen sollten. In einigen Fällen müssen Sie eines der Objekte in Konflikt zu löschen.
    
4. Wenn Sie die Änderung in die lokale Active Directory vorgenommen, lassen Sie Azure AD-Connect synchronisieren Sie die Änderung für den Fehler behoben werden.
    

