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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="addb4-102">ConsistencyGuid/sourceAnchor-Verhalten</span><span class="sxs-lookup"><span data-stu-id="addb4-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="addb4-103">Azure AD Connect (Version 1.1.524.0 und nach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut.</span><span class="sxs-lookup"><span data-stu-id="addb4-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="addb4-104">Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für:</span><span class="sxs-lookup"><span data-stu-id="addb4-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="addb4-105">Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte.</span><span class="sxs-lookup"><span data-stu-id="addb4-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="addb4-106">ObjectGUID wird für andere Objekttypen verwendet.</span><span class="sxs-lookup"><span data-stu-id="addb4-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="addb4-107">Für jedes lokale AD User-Objekt, dessen msDS-ConsistencyGuid-Attribut nicht aufgefüllt wird, schreibt Azure AD Connect seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="addb4-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="addb4-108">Nachdem das attribut msDS-ConsistencyGuid aufgefüllt wurde, exportiert Azure AD Connect das Objekt dann nach Azure AD.</span><span class="sxs-lookup"><span data-stu-id="addb4-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="addb4-109">**Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (d. h. in den AD Connector Space importiert und in das Metaverse projiziert wurde), können Sie seinen sourceAnchor-Wert nicht mehr ändern.</span><span class="sxs-lookup"><span data-stu-id="addb4-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="addb4-110">Um den sourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie sein msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Connect importiert wird.</span><span class="sxs-lookup"><span data-stu-id="addb4-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="addb4-111">Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie im Folgenden: [Azure AD Connect: Entwurfskonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="addb4-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

