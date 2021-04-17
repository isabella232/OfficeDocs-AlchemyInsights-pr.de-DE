---
title: ConsistencyGuid/sourceAnchor-Verhalten
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816991"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-Verhalten

Azure AD Connect (Version 1.1.524.0 und nach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für:
  
- Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für jedes lokale AD User-Objekt, dessen msDS-ConsistencyGuid-Attribut nicht aufgefüllt wird, schreibt Azure AD Connect seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory. Nachdem das attribut msDS-ConsistencyGuid aufgefüllt wurde, exportiert Azure AD Connect das Objekt dann nach Azure AD.
    
 **Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (d. h. in den AD Connector Space importiert und in das Metaverse projiziert wurde), können Sie seinen sourceAnchor-Wert nicht mehr ändern. Um den sourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie sein msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Connect importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie im Folgenden: [Azure AD Connect: Entwurfskonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

