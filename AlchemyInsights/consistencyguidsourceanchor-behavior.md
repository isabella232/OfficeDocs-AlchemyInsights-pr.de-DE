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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516979"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/Attributs-Verhalten

Azure AD Connect (Version 1.1.524.0 und After) erleichtert jetzt die Verwendung von MSDS-ConsistencyGuid als Attributs-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für Folgendes:
  
- Verwenden Sie MSDS-ConsistencyGuid als Attributs-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für ein bestimmtes lokales AD-Benutzerobjekt, dessen MSDS-ConsistencyGuid-Attribut nicht aufgefüllt wird, schreibt Azure AD Connect den Wert der objectGUID zurück in das msDS-ConsistencyGuid-Attribut in der lokalen Active Directory. Nachdem das msDS-ConsistencyGuid-Attribut aufgefüllt wurde, exportiert Azure AD Connect das Objekt dann in Azure AD.
    
 **Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (also in den AD Connector-Speicher importiert und in das Metaverse projiziert wurde), können Sie den Attributs-Wert nicht mehr ändern. Um den Attributs-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das zugehörige MSDS-ConsistencyGuid-Attribut, bevor es in Azure AD Connect importiert wird. 
  
Weitere Informationen zu Attributs und ConsistencyGuid finden Sie in den folgenden Themen: [Azure AD Connect: Design Concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

