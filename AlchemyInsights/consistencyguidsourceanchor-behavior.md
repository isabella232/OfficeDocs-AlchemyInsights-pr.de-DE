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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516979"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="fe611-102">ConsistencyGuid/Attributs-Verhalten</span><span class="sxs-lookup"><span data-stu-id="fe611-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="fe611-103">Azure AD Connect (Version 1.1.524.0 und After) erleichtert jetzt die Verwendung von MSDS-ConsistencyGuid als Attributs-Attribut.</span><span class="sxs-lookup"><span data-stu-id="fe611-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="fe611-104">Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="fe611-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="fe611-105">Verwenden Sie MSDS-ConsistencyGuid als Attributs-Attribut für User-Objekte.</span><span class="sxs-lookup"><span data-stu-id="fe611-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="fe611-106">ObjectGUID wird für andere Objekttypen verwendet.</span><span class="sxs-lookup"><span data-stu-id="fe611-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="fe611-107">Für ein bestimmtes lokales AD-Benutzerobjekt, dessen MSDS-ConsistencyGuid-Attribut nicht aufgefüllt wird, schreibt Azure AD Connect den Wert der objectGUID zurück in das msDS-ConsistencyGuid-Attribut in der lokalen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fe611-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="fe611-108">Nachdem das msDS-ConsistencyGuid-Attribut aufgefüllt wurde, exportiert Azure AD Connect das Objekt dann in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe611-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="fe611-109">**Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (also in den AD Connector-Speicher importiert und in das Metaverse projiziert wurde), können Sie den Attributs-Wert nicht mehr ändern.</span><span class="sxs-lookup"><span data-stu-id="fe611-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="fe611-110">Um den Attributs-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das zugehörige MSDS-ConsistencyGuid-Attribut, bevor es in Azure AD Connect importiert wird.</span><span class="sxs-lookup"><span data-stu-id="fe611-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="fe611-111">Weitere Informationen zu Attributs und ConsistencyGuid finden Sie in den folgenden Themen: [Azure AD Connect: Design Concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="fe611-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

