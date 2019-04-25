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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408107"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="1f7da-102">ConsistencyGuid/Attributs-Verhalten</span><span class="sxs-lookup"><span data-stu-id="1f7da-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="1f7da-103">Azure AD Connect (Version 1.1.524.0 und nachher) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als Attributs-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1f7da-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="1f7da-104">Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="1f7da-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="1f7da-105">Verwenden Sie msDS-ConsistencyGuid als Attributs-Attribut für Benutzerobjekte.</span><span class="sxs-lookup"><span data-stu-id="1f7da-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="1f7da-106">ObjectGUID wird für andere Objekttypen verwendet.</span><span class="sxs-lookup"><span data-stu-id="1f7da-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="1f7da-107">Für ein lokales AD-Benutzerobjekt, dessen msDS-ConsistencyGuid-Attribut nicht aufgefüllt wird, schreibt Azure AD Connect seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1f7da-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="1f7da-108">Nachdem das msDS-ConsistencyGuid-Attribut aufgefüllt wurde, wird das Objekt von Azure AD Connect in Azure AD exportiert.</span><span class="sxs-lookup"><span data-stu-id="1f7da-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="1f7da-109">**Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (das in den AD-Connector-Bereich importiert und in das Metaverse projiziert wurde), kann der Attributs-Wert nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="1f7da-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="1f7da-110">Um den Attributs-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie sein msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Connect importiert wird.</span><span class="sxs-lookup"><span data-stu-id="1f7da-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="1f7da-111">Weitere Informationen zu Attributs und ConsistencyGuid finden Sie im folgenden Thema: [Azure AD Connect: Design Concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="1f7da-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

