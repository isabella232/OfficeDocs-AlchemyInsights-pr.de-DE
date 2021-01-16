---
title: Domänendienstsynchronisierung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876516"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="fd5ef-102">Domänendienstsynchronisierung</span><span class="sxs-lookup"><span data-stu-id="fd5ef-102">Domain service synchronization</span></span>

<span data-ttu-id="fd5ef-103">Objekte und Anmeldeinformationen in einer verwalteten Azure Active Directory Domain Services (Azure AD DS)-Domäne können entweder lokal innerhalb der Domäne erstellt oder von einem Azure Active Directory (Azure AD)-Mandanten synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="fd5ef-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="fd5ef-104">Bei der ersten Bereitstellung von Azure AD DS wird eine automatische one-way-Synchronisierung konfiguriert und initiiert, um die Objekte aus Azure AD zu replizieren.</span><span class="sxs-lookup"><span data-stu-id="fd5ef-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="fd5ef-105">Diese one-way-Synchronisierung wird weiterhin im Hintergrund ausgeführt, um die von Azure AD DS verwaltete Domäne mit allen Änderungen von Azure AD auf dem neuesten Stand zu halten.</span><span class="sxs-lookup"><span data-stu-id="fd5ef-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="fd5ef-106">Es erfolgt keine Synchronisierung von Azure AD DS zurück zu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd5ef-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="fd5ef-107">Weitere Informationen zur Synchronisierung des Azure Active Directory-Domänendiensts finden Sie unter [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="fd5ef-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
