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
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659590"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="fa0ad-102">ConsistencyGuid / SourceAnchor-Verhalten</span><span class="sxs-lookup"><span data-stu-id="fa0ad-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="fa0ad-p101">Azure Active Directory verbinden (Version 1.1.524.0 und nach) jetzt erleichtert die Verwendung von MsDS-ConsistencyGuid als SourceAnchor-Attribut. Wenn Sie dieses Feature verwenden, konfiguriert Azure AD-Connect automatisch die Synchronisierungsregeln an:</span><span class="sxs-lookup"><span data-stu-id="fa0ad-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="fa0ad-p102">Verwenden Sie MsDS-ConsistencyGuid als SourceAnchor-Attribut für User-Objekte. Objekt-GUID wird für andere Objekttypen verwendet.</span><span class="sxs-lookup"><span data-stu-id="fa0ad-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="fa0ad-p103">Für eine bestimmte lokale Active Directory-Benutzer, deren Attribut MsDS-ConsistencyGuid ist nicht gefüllt, Azure AD-Connect Schreibvorgänge der Objekt-GUID-Wert zurück, an das Attribut MsDS-ConsistencyGuid im lokalen Active Directory-Objekt. Nachdem das Attribut MsDS-ConsistencyGuid aufgefüllt wird, exportiert Azure AD-Connect das Objekt dann in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fa0ad-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="fa0ad-p104">**Hinweis:** Einmal einem lokalen AD-Objekt wird in Azure AD-Connect (das ist, in den Connectorbereich AD importiert und in der Metaverse projiziert) importiert, SourceAnchor Wert nicht mehr ändern. Zum Angeben des SourceAnchor Werts für einen angegebenen lokalen AD-Objekts, das Attribut MsDS-ConsistencyGuid konfigurieren, bevor er in Azure AD-Connect importiert wird.</span><span class="sxs-lookup"><span data-stu-id="fa0ad-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="fa0ad-111">Weitere Informationen zu SourceAnchor und ConsistencyGuid, finden Sie in den folgenden: [Azure AD-Connect: Entwerfen Konzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="fa0ad-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

