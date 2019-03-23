---
title: ConsistencyGuid/Attributs-Verhalten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753101"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/Attributs-Verhalten

Azure AD Connect (Version 1.1.524.0 und nachher) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als Attributs-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für Folgendes:
  
- Verwenden Sie msDS-ConsistencyGuid als Attributs-Attribut für Benutzerobjekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für ein lokales AD-Benutzerobjekt, dessen msDS-ConsistencyGuid-Attribut nicht aufgefüllt wird, schreibt Azure AD Connect seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory. Nachdem das msDS-ConsistencyGuid-Attribut aufgefüllt wurde, wird das Objekt von Azure AD Connect in Azure AD exportiert.
    
 **Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (das in den AD-Connector-Bereich importiert und in das Metaverse projiziert wurde), kann der Attributs-Wert nicht mehr geändert werden. Um den Attributs-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie sein msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Connect importiert wird. 
  
Weitere Informationen zu Attributs und ConsistencyGuid finden Sie im folgenden Thema: [Azure AD Connect: Design Concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

