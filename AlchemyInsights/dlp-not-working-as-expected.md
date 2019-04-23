---
title: DLP funktioniert nicht wie erwartet
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 6d8e3e540494e99e42f04080681f46324f2936bd
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2019
ms.locfileid: "31869558"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="92f5c-102">DLP funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="92f5c-102">DLP not working as expected</span></span>


<span data-ttu-id="92f5c-103">Haben Sie Probleme mit dem **Schutz vor Datenverlust (DLP)** in Office 365, die nicht wie erwartet funktionieren?</span><span class="sxs-lookup"><span data-stu-id="92f5c-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="92f5c-104">Stellen Sie in diesem Fall sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, was die **DLP-Richtlinie** bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="92f5c-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="92f5c-105">**Einrichten von DLP:**</span><span class="sxs-lookup"><span data-stu-id="92f5c-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="92f5c-106">Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="92f5c-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="92f5c-107">Verwenden Sie zum Einrichten von DLP-Richtlinien die Informationen [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="92f5c-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="92f5c-108">**Wonach die DLP-Richtlinien aussehen:**</span><span class="sxs-lookup"><span data-stu-id="92f5c-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="92f5c-109">Bei Verwendung der **integrierten vertraulichen Informationstypen** in Office 365 Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn Sie diese vertraulichen Typen erkennen.</span><span class="sxs-lookup"><span data-stu-id="92f5c-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="92f5c-110">**Integrierte Typen von vertraulichen Informationen:**</span><span class="sxs-lookup"><span data-stu-id="92f5c-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="92f5c-111">Informationen zu den integrierten vertraulichen Typen und den Anforderungen einer DLP-Richtlinie bei der Ermittlung des vertraulichen Typs finden Sie unter: [wonach die Typen von vertraulichen Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="92f5c-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="92f5c-112">**Benutzerdefinierte Typen für vertrauliche Informationen:**</span><span class="sxs-lookup"><span data-stu-id="92f5c-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="92f5c-113">Wenn Sie versuchen, benutzerdefinierte Typen für vertrauliche Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="92f5c-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="92f5c-114">**Berichte**</span><span class="sxs-lookup"><span data-stu-id="92f5c-114">**Reports:**</span></span>
  
- <span data-ttu-id="92f5c-115">Holen Sie sich vertrauliche Daten mit [DLP-Berichten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="92f5c-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="92f5c-116">Details des Ereignisses mit einem [Vorfall Bericht](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)anzeigen.</span><span class="sxs-lookup"><span data-stu-id="92f5c-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    

