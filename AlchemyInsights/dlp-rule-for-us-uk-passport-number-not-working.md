---
title: DLP-Regel für US / Großbritannien Reisepassnummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912096"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="15aa7-102">Probleme mit DLP - US / Ausweisnummern Großbritannien</span><span class="sxs-lookup"><span data-stu-id="15aa7-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="15aa7-p101">Haben Sie Probleme mit **Data Loss Prevention (DLP)** funktioniert nicht für Inhalt mit einer **US / Großbritannien Reisepassnummer** bei Verwendung eines DLP-Typs vertraulicher Informationen in Office 365? In diesem Fall enthält stellen Sie sicher, dass Ihre Inhalte die erforderliche Informationen für welche die DLP-Richtlinie Ansichtsseite sucht bei der Auswertung.</span><span class="sxs-lookup"><span data-stu-id="15aa7-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="15aa7-105">Beispiel für eine **US / Großbritannien Reisepassnummer** mit einer Vertrauensstufe von 75 % konfigurierte Richtlinie, die folgenden ausgewertet werden und muss für die Regel ausgelöst erkannt werden</span><span class="sxs-lookup"><span data-stu-id="15aa7-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="15aa7-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neun Ziffern</span><span class="sxs-lookup"><span data-stu-id="15aa7-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="15aa7-107">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neun aufeinander folgenden Ziffern</span><span class="sxs-lookup"><span data-stu-id="15aa7-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="15aa7-108">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, keine Prüfsumme vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15aa7-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="15aa7-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Eine DLP-Richtlinie ist 75 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="15aa7-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="15aa7-110">Die Funktion Func_usa_uk_passport findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="15aa7-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="15aa7-111">Ein Schlüsselwort aus Keyword_passport wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="15aa7-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="15aa7-112">Im folgende Beispiel würden beispielsweise trigger für die **US / Großbritannien Reisepassnummer** Richtlinie: US Reisepassnummer 123456789</span><span class="sxs-lookup"><span data-stu-id="15aa7-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="15aa7-113">Weitere Informationen zu für eine US Anforderungen / Großbritannien Reisepassnummer für Ihre Inhalte erkannt werden, finden Sie unter den folgenden Abschnitt in diesem Artikel: [was der vertraulichen Informationstypen Darstellung für US / Großbritannien Reisepassnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="15aa7-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="15aa7-114">Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="15aa7-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

