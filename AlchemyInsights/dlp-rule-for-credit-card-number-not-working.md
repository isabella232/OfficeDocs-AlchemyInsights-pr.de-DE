---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389576"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="686ea-102">DLP-Probleme mit Kreditkartennummern</span><span class="sxs-lookup"><span data-stu-id="686ea-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="686ea-103">Haben Sie Probleme mit der Verhinderung von **Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **Kreditkartennummer** funktioniert?</span><span class="sxs-lookup"><span data-stu-id="686ea-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="686ea-104">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn Sie ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="686ea-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="686ea-105">Für eine **Kreditkarten Richtlinie** , die mit einer Konfidenz Stufe von 85% konfiguriert ist, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="686ea-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="686ea-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddddddddddddddd) sein können und den Luhn-Test bestehen müssen.</span><span class="sxs-lookup"><span data-stu-id="686ea-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="686ea-107">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplexes und robustes Muster, das Karten von allen wichtigen Marken weltweit erkennt, einschließlich Visa, Mastercard, Discover Card, JCB, American Express, Geschenkkarten und Diner Cards.</span><span class="sxs-lookup"><span data-stu-id="686ea-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="686ea-108">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Luhn-Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="686ea-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="686ea-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="686ea-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="686ea-110">Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="686ea-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="686ea-111">Eine der folgenden Bedingungen trifft zu:</span><span class="sxs-lookup"><span data-stu-id="686ea-111">One of the following is true:</span></span>

  - <span data-ttu-id="686ea-112">Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="686ea-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="686ea-113">Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="686ea-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="686ea-114">Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.</span><span class="sxs-lookup"><span data-stu-id="686ea-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="686ea-115">Die Prüfsummen Übergabe</span><span class="sxs-lookup"><span data-stu-id="686ea-115">The checksum passes</span></span>

    <span data-ttu-id="686ea-116">Beispielsweise würde das folgende Beispiel für eine DLP-Kreditkartennummern Richtlinie ausgelöst werden:</span><span class="sxs-lookup"><span data-stu-id="686ea-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="686ea-117">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="686ea-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="686ea-118">Gültig bis: 2/2009</span><span class="sxs-lookup"><span data-stu-id="686ea-118">Expires: 2/2009</span></span>

<span data-ttu-id="686ea-119">Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für Kreditkarte suchen #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="686ea-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="686ea-120">Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="686ea-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  