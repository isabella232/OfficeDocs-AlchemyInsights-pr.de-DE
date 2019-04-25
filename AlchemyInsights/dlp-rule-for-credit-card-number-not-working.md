---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404493"
---
<span data-ttu-id="cf309-102">Haben Sie Probleme mit **Data Loss Prevention (DLP)** , die nicht für Inhalte, die eine **Kreditkartennummer** enthalten, bei Verwendung eines DLP-vertraulichen Informationstyps in O365?</span><span class="sxs-lookup"><span data-stu-id="cf309-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="cf309-103">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn Sie ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="cf309-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="cf309-104">Bei einer **Kreditkarten Richtlinie** , die mit einem Konfidenzniveau von 85% konfiguriert wurde, werden beispielsweise folgende Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="cf309-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="cf309-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddddddddddddddd) werden können und den Luhn-Test bestehen müssen.</span><span class="sxs-lookup"><span data-stu-id="cf309-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="cf309-106">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplexes und robustes Muster, das Karten aller wichtigen Marken weltweit erkennt, einschließlich Visa, MasterCard, Discover Card, JCB, American Express, Geschenkkarten und dinerkarten.</span><span class="sxs-lookup"><span data-stu-id="cf309-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="cf309-107">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Luhn-Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="cf309-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="cf309-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85% sicher, dass Sie diese Art von vertraulichen Informationen erkannt hat, wenn Sie innerhalb einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="cf309-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="cf309-109">Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="cf309-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="cf309-110">Eine der folgenden Bedingungen trifft zu:</span><span class="sxs-lookup"><span data-stu-id="cf309-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="cf309-111">Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="cf309-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="cf309-112">Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="cf309-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="cf309-113">Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.</span><span class="sxs-lookup"><span data-stu-id="cf309-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="cf309-114">Die Prüfsumme wird übergeben.</span><span class="sxs-lookup"><span data-stu-id="cf309-114">The checksum passes</span></span>
    
    <span data-ttu-id="cf309-115">Das folgende Beispiel würde beispielsweise für eine DLP-Kreditkartennummern Richtlinie auslösen:</span><span class="sxs-lookup"><span data-stu-id="cf309-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="cf309-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="cf309-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="cf309-117">Expires: 2/2009</span><span class="sxs-lookup"><span data-stu-id="cf309-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="cf309-118">Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt dieses Artikels: [was die Typen vertraulicher Informationen für Kreditkartennummern suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="cf309-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="cf309-119">Verwenden Sie einen anderen integrierten vertraulichen Informationstyp, um Informationen darüber zu erhalten, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="cf309-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

