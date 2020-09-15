---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679440"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="c4dff-102">DLP-Probleme mit Kreditkartennummern</span><span class="sxs-lookup"><span data-stu-id="c4dff-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="c4dff-103">**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="c4dff-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c4dff-104">**DLP-Probleme mit Kreditkartennummern**</span><span class="sxs-lookup"><span data-stu-id="c4dff-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="c4dff-105">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **Kreditkartennummer** funktioniert?</span><span class="sxs-lookup"><span data-stu-id="c4dff-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c4dff-106">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn Sie ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="c4dff-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="c4dff-107">Für eine **Kreditkarten Richtlinie** , die mit einer Konfidenz Stufe von 85% konfiguriert ist, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="c4dff-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c4dff-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddddddddddddddd) sein können und den Luhn-Test bestehen müssen.</span><span class="sxs-lookup"><span data-stu-id="c4dff-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="c4dff-109">**[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Sehr komplexes und robustes Muster, das Karten von allen wichtigen Marken weltweit erkennt, einschließlich Visa, Mastercard, Discover Card, JCB, American Express, Geschenkkarten und Diner Cards.</span><span class="sxs-lookup"><span data-stu-id="c4dff-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="c4dff-110">**[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, die Luhn-Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="c4dff-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="c4dff-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Eine DLP-Richtlinie ist 85% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="c4dff-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c4dff-112">Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="c4dff-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c4dff-113">Eine der folgenden Bedingungen trifft zu:</span><span class="sxs-lookup"><span data-stu-id="c4dff-113">One of the following is true:</span></span>

  - <span data-ttu-id="c4dff-114">Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="c4dff-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="c4dff-115">Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="c4dff-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="c4dff-116">Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.</span><span class="sxs-lookup"><span data-stu-id="c4dff-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="c4dff-117">Die Prüfsummen Übergabe</span><span class="sxs-lookup"><span data-stu-id="c4dff-117">The checksum passes</span></span>

    <span data-ttu-id="c4dff-118">Beispielsweise würde das folgende Beispiel für eine DLP-Kreditkartennummern Richtlinie ausgelöst werden:</span><span class="sxs-lookup"><span data-stu-id="c4dff-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="c4dff-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="c4dff-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="c4dff-120">Gültig bis: 2/2009</span><span class="sxs-lookup"><span data-stu-id="c4dff-120">Expires: 2/2009</span></span>

<span data-ttu-id="c4dff-121">Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für Kreditkarte suchen #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="c4dff-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="c4dff-122">Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c4dff-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  