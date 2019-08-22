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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504993"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e9501-102">Bedingter Zugriff mit InTune</span><span class="sxs-lookup"><span data-stu-id="e9501-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e9501-103">Die Verwendung von **bedingtem Zugriff** mit InTune erfordert 3 Schritte:</span><span class="sxs-lookup"><span data-stu-id="e9501-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e9501-104">Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="e9501-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="e9501-105">Beispielsweise muss ein Gerät kompatibel sein, bevor auf Firmen-e-Mails zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="e9501-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e9501-106">Erstellen Sie eine **Konformitätsrichtlinie** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als konform betrachtet wird.</span><span class="sxs-lookup"><span data-stu-id="e9501-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e9501-107">Ein Gerät muss beispielsweise eine PIN von mindestens 6 Ziffern aufweisen, bevor es als konform gilt.</span><span class="sxs-lookup"><span data-stu-id="e9501-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e9501-108">Sicherstellen, dass sowohl **Compliance-Richt** Linien als auch **Richtlinien für bedingten Zugriff** auf die gewünschten Benutzergruppen zugeschnitten sind.</span><span class="sxs-lookup"><span data-stu-id="e9501-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="e9501-109">Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e9501-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e9501-110">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="e9501-110">Read more:</span></span>
  
- [<span data-ttu-id="e9501-111">Bewährte Methoden für bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="e9501-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e9501-112">Erste Schritte mit bedingtem Zugriff</span><span class="sxs-lookup"><span data-stu-id="e9501-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

