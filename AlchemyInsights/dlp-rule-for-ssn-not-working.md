---
title: DLP-Regel für SSN nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289187"
---
<span data-ttu-id="57560-p101">Haben Sie Probleme mit der **Data Loss Prevention (DLP)** für Inhalte mit einer **Sozialversicherungsnummer (SSN)** , wenn ein anderes vertrauliche Informationen in Office 365 verwenden nicht ordnungsgemäß ausgeführt? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte enthält die erforderliche Informationen für die DLP-Richtlinie suchen.</span><span class="sxs-lookup"><span data-stu-id="57560-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="57560-104">Beispiel für eine SSN-Richtlinie mit einer Vertrauensstufe von 85 % konfiguriert, die folgenden ausgewertet werden und müssen erkannt werden, für die Regel ausgelöst:</span><span class="sxs-lookup"><span data-stu-id="57560-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="57560-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 Ziffern, die in einem Muster formatierte oder unformatierte sein können</span><span class="sxs-lookup"><span data-stu-id="57560-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="57560-106">**[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier Funktionen suchen SSNs in vier verschiedene Muster:</span><span class="sxs-lookup"><span data-stu-id="57560-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="57560-107">Func_ssn sucht nach US-Sozialversicherungsnummern von vor 2011, die mithilfe von Bindestrichen oder Leerzeichen (ddd-dd-dddd ODER ddd dd dddd) formatiert sind </span><span class="sxs-lookup"><span data-stu-id="57560-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="57560-108">Func_unformatted_ssn sucht nach US-Sozialversicherungnummern von vor 2011, die als neun aufeinander folgende Ziffern (ddddddddd) formatiert sind</span><span class="sxs-lookup"><span data-stu-id="57560-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="57560-109">Func_randomized_formatted_ssn sucht nach US-Sozialversicherungsnummern von nach 2011, die mithilfe von Bindestrichen oder Leerzeichen (ddd-dd-dddd ODER ddd dd dddd) formatiert sind </span><span class="sxs-lookup"><span data-stu-id="57560-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="57560-110">Func_randomized_unformatted_ssn sucht nach US-Sozialversicherungnummern von nach 2011, die als neun aufeinander folgende Ziffern (ddddddddd) formatiert sind</span><span class="sxs-lookup"><span data-stu-id="57560-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="57560-111">**[Prüfsumme:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nein, keine Prüfsumme vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="57560-111">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="57560-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Eine DLP-Richtlinie ist 85 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="57560-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="57560-113">Die [Funktion Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) sucht nach Inhalten, die dem Muster entspricht.</span><span class="sxs-lookup"><span data-stu-id="57560-113">The [function Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="57560-p102">Ein Schlüsselwort aus [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) gefunden wird. Enthält Beispiele für Schlüsselwörter: *soziale Sicherheit, Sozialleistungen #, Krankenversicherung, SSN* . Beispielsweise würde im folgende Beispiel für die SSN DLP-Richtlinie ausgelöst: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="57560-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="57560-117">Weitere Informationen zu Anforderungen für SSNs für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Was der vertraulichen Informationstypen SSNs suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="57560-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="57560-118">Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="57560-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

