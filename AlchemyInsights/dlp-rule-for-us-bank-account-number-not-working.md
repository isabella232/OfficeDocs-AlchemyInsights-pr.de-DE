---
title: DLP-Regel für US-Kontonummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404268"
---
<span data-ttu-id="34b3b-102">Haben Sie Probleme mit dem **Schutz vor Datenverlust (DLP)** , die für Inhalte, die eine **US-Bank Kontonummer** enthalten, nicht arbeiten, wenn Sie einen DLP-vertraulichen Informationstyp in O365 verwenden?</span><span class="sxs-lookup"><span data-stu-id="34b3b-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="34b3b-103">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für die Anforderungen der DLP-Richtlinie bei der Auswertung enthalten.</span><span class="sxs-lookup"><span data-stu-id="34b3b-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="34b3b-104">Bei einer Richtlinie mit **US-Kontonummern** , die mit einem Konfidenzniveau von 85% konfiguriert wurde, werden beispielsweise folgende Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="34b3b-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="34b3b-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 Ziffern</span><span class="sxs-lookup"><span data-stu-id="34b3b-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="34b3b-106">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 aufeinanderfolgende Ziffern.</span><span class="sxs-lookup"><span data-stu-id="34b3b-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="34b3b-107">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, es gibt keine prüfSumme</span><span class="sxs-lookup"><span data-stu-id="34b3b-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="34b3b-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Eine DLP-Richtlinie ist 75% sicher, dass Sie diese Art von vertraulichen Informationen erkannt hat, wenn Sie innerhalb einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="34b3b-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="34b3b-109">Der reguläre Ausdruck Regex_usa_bank_account_number findet Inhalte, die mit dem Muster übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="34b3b-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="34b3b-110">Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="34b3b-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="34b3b-111">Das folgende Beispiel würde beispielsweise für die US-Konto **Nummern** Richtlinie auslösen: girokonto 78344011</span><span class="sxs-lookup"><span data-stu-id="34b3b-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="34b3b-112">Weitere Informationen dazu, was erforderlich ist, damit eine **US-Bank Kontonummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt dieses Artikels: [was die Typen vertraulicher Informationen für die US-Bankkontonummer suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="34b3b-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="34b3b-113">Verwenden Sie einen anderen integrierten vertraulichen Informationstyp, um Informationen darüber zu erhalten, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="34b3b-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

