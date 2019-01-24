---
title: Bedingte Zugriff mit Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470356"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ed0a1-102">Bedingte Zugriff mit Intune</span><span class="sxs-lookup"><span data-stu-id="ed0a1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ed0a1-103">Verwenden von **Bedingten Zugriff** mit Intune sind 3 Schritte erforderlich:</span><span class="sxs-lookup"><span data-stu-id="ed0a1-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ed0a1-p101">Erstellen Sie eine **Bedingte Zugriffsrichtlinie** , die definiert, welche Ressourcen geschützt sind und welche Bedingungen müssen erfüllt sein, um diese Ressourcen zuzugreifen. Vor dem Zugriff auf Unternehmens-e-Mail-muss beispielsweise ein Gerät kompatibel sein.</span><span class="sxs-lookup"><span data-stu-id="ed0a1-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ed0a1-p102">Erstellen einer **Compliance-Richtlinien** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät kompatibel ist. Beispielsweise muss ein Gerät eine PIN-Nummer der mindestens 6 Stellen aufweisen, bevor kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="ed0a1-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ed0a1-p103">Sicherstellen, dass **Kompatibilitätsrichtlinien** und **Bedingte Zugriffsrichtlinien** geplant, um die gewünschten Benutzergruppen. Dies erfordert möglicherweise bestimmte Gruppen von Benutzern in Azure Active Directory erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed0a1-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ed0a1-110">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="ed0a1-110">Read more:</span></span>
  
- [<span data-ttu-id="ed0a1-111">Bedingte Access bewährte Methoden</span><span class="sxs-lookup"><span data-stu-id="ed0a1-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ed0a1-112">Erste Schritte mit bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="ed0a1-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

