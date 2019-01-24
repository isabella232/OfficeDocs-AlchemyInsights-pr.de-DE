---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470501"
---
<span data-ttu-id="12bd4-p101">Haben Sie Probleme mit der **Data Loss Prevention (DLP)** funktioniert nicht für Inhalt mit einer **Kreditkartennummer** , wenn ein anderes DLP vertrauliche Informationen in Office 365 verwenden? Wenn dies der Fall ist, stellen Sie sicher, Ihre Inhalte enthält die erforderliche Informationen zum Auslösen der DLP-Richtlinie, wenn sie ausgewertet wird. Beispiel für eine **Kreditkarte Richtlinie** mit einer Vertrauensstufe von 85 % konfiguriert, die folgenden ausgewertet werden und erkannt werden muss, für die Regel ausgelöst:</span><span class="sxs-lookup"><span data-stu-id="12bd4-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="12bd4-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Stellen die formatiert werden können oder unformatierte (Dddddddddddddddd), und geben Sie den Test mit Luhn müssen.</span><span class="sxs-lookup"><span data-stu-id="12bd4-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="12bd4-106">**[Muster:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplex und robuste Muster, das Karten aus alle wichtigen Marken weltweit, einschließlich Visa, Mastercard, Discover-Karte, JCB, amerikanische Express, Geschenkgutscheine und Bestellung Karten erkennt.</span><span class="sxs-lookup"><span data-stu-id="12bd4-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="12bd4-107">**[Prüfsumme:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Prüfsumme Luhn</span><span class="sxs-lookup"><span data-stu-id="12bd4-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="12bd4-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="12bd4-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="12bd4-109">Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="12bd4-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="12bd4-110">Eine der folgenden Bedingungen trifft zu:</span><span class="sxs-lookup"><span data-stu-id="12bd4-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="12bd4-111">Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="12bd4-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="12bd4-112">Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="12bd4-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="12bd4-113">Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.</span><span class="sxs-lookup"><span data-stu-id="12bd4-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="12bd4-114">Die Prüfsumme stimmt.</span><span class="sxs-lookup"><span data-stu-id="12bd4-114">The checksum passes</span></span>
    
    <span data-ttu-id="12bd4-115">Beispielsweise würde im folgende Beispiel für eine DLP Kreditkarte Anzahl Richtlinie ausgelöst:</span><span class="sxs-lookup"><span data-stu-id="12bd4-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="12bd4-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="12bd4-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="12bd4-117">Gültig bis: 2/2009</span><span class="sxs-lookup"><span data-stu-id="12bd4-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="12bd4-118">Weitere Informationen zu Anforderungen für eine **Kreditkartennummer** für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Was der vertraulichen Informationstypen für Kreditkarte-suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="12bd4-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="12bd4-119">Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="12bd4-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

