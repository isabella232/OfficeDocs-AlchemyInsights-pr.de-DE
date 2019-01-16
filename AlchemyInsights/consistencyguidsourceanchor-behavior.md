---
title: ConsistencyGuid / SourceAnchor-Verhalten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289329"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / SourceAnchor-Verhalten

Azure Active Directory verbinden (Version 1.1.524.0 und nach) jetzt erleichtert die Verwendung von MsDS-ConsistencyGuid als SourceAnchor-Attribut. Wenn Sie dieses Feature verwenden, konfiguriert Azure AD-Connect automatisch die Synchronisierungsregeln an:
  
- Verwenden Sie MsDS-ConsistencyGuid als SourceAnchor-Attribut für User-Objekte. Objekt-GUID wird für andere Objekttypen verwendet.
    
- Für eine bestimmte lokale Active Directory-Benutzer, deren Attribut MsDS-ConsistencyGuid ist nicht gefüllt, Azure AD-Connect Schreibvorgänge der Objekt-GUID-Wert zurück, an das Attribut MsDS-ConsistencyGuid im lokalen Active Directory-Objekt. Nachdem das Attribut MsDS-ConsistencyGuid aufgefüllt wird, exportiert Azure AD-Connect das Objekt dann in Azure AD.
    
 **Hinweis:** Einmal einem lokalen AD-Objekt wird in Azure AD-Connect (das ist, in den Connectorbereich AD importiert und in der Metaverse projiziert) importiert, SourceAnchor Wert nicht mehr ändern. Zum Angeben des SourceAnchor Werts für einen angegebenen lokalen AD-Objekts, das Attribut MsDS-ConsistencyGuid konfigurieren, bevor er in Azure AD-Connect importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid, finden Sie in den folgenden: [Azure AD-Connect: Entwerfen Konzepte](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

