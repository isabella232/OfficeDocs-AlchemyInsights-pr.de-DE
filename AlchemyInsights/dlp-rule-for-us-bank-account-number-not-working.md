---
title: DLP-Regel für uns Bankkontonummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290261"
---
<span data-ttu-id="e7216-p101">Haben Sie Probleme mit der **Data Loss Prevention (DLP)** funktioniert nicht für Inhalt mit einer **Kontonummer US** , wenn ein anderes DLP vertrauliche Informationen in Office 365 verwenden? In diesem Fall enthält stellen Sie sicher, dass Ihre Inhalte die erforderliche Informationen für welche die DLP-Richtlinie Ansichtsseite sucht bei der Auswertung.</span><span class="sxs-lookup"><span data-stu-id="e7216-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="e7216-104">Beispiel für eine **Kontonummer US** -Richtlinie mit einer Vertrauensstufe von 85 % konfiguriert, die folgenden ausgewertet werden und müssen erkannt werden, für die Regel ausgelöst:</span><span class="sxs-lookup"><span data-stu-id="e7216-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="e7216-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 bis 17 Ziffern</span><span class="sxs-lookup"><span data-stu-id="e7216-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="e7216-106">**[Muster:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 bis 17 aufeinander folgenden Ziffern.</span><span class="sxs-lookup"><span data-stu-id="e7216-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="e7216-107">**[Prüfsumme:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, keine Prüfsumme vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="e7216-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="e7216-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Eine DLP-Richtlinie ist 75 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="e7216-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e7216-109">Der reguläre Ausdruck Regex_usa_bank_account_number sucht nach Inhalten, die dem Muster entspricht</span><span class="sxs-lookup"><span data-stu-id="e7216-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="e7216-110">Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="e7216-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="e7216-111">Beispielsweise würde im folgende Beispiel für die **USA Bankkontonummer** Richtlinie ausgelöst: Bankkonto 78344011</span><span class="sxs-lookup"><span data-stu-id="e7216-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="e7216-112">Weitere Informationen zu Anforderungen für eine **Kontonummer US** für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Was der vertraulichen Informationstypen US Bankkontonummer suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="e7216-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="e7216-113">Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e7216-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

