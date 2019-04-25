---
title: Bedingter Zugriff mit InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393540"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="4cf94-102">Bedingter Zugriff mit InTune</span><span class="sxs-lookup"><span data-stu-id="4cf94-102">Conditional Access with Intune</span></span>

<span data-ttu-id="4cf94-103">Die Verwendung des **bedingten Zugriffs** mit InTune erfordert drei Schritte:</span><span class="sxs-lookup"><span data-stu-id="4cf94-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="4cf94-104">Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zugreifen zu können.</span><span class="sxs-lookup"><span data-stu-id="4cf94-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="4cf94-105">Ein Gerät muss beispielsweise vor dem Zugriff auf geschäftliche e-Mails kompatibel sein.</span><span class="sxs-lookup"><span data-stu-id="4cf94-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="4cf94-106">Erstellen Sie eine **Konformitätsrichtlinie** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als kompatibel eingestuft wird.</span><span class="sxs-lookup"><span data-stu-id="4cf94-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="4cf94-107">Ein Gerät muss beispielsweise über eine PIN von mindestens 6 Ziffern verfügen, bevor es als kompatibel angesehen wird.</span><span class="sxs-lookup"><span data-stu-id="4cf94-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="4cf94-108">Sicherstellen, dass sowohl **Konformitätsrichtlinien** als auch **Richtlinien für den bedingten Zugriff** für die gewünschten Benutzergruppen vorgesehen sind.</span><span class="sxs-lookup"><span data-stu-id="4cf94-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="4cf94-109">Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4cf94-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="4cf94-110">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="4cf94-110">Read more:</span></span>
  
- [<span data-ttu-id="4cf94-111">Bewährte Methoden für bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="4cf94-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="4cf94-112">Erste Schritte mit bedingtem Zugriff</span><span class="sxs-lookup"><span data-stu-id="4cf94-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

