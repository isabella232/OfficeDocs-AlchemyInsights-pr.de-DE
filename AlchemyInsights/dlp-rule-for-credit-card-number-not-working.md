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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932442"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="ab515-102">DLP-Probleme mit Kreditkartennummern</span><span class="sxs-lookup"><span data-stu-id="ab515-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="ab515-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="ab515-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ab515-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="ab515-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ab515-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="ab515-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ab515-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="ab515-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ab515-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="ab515-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ab515-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="ab515-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ab515-109">**DLP-Probleme mit Kreditkartennummern**</span><span class="sxs-lookup"><span data-stu-id="ab515-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="ab515-110">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **Kreditkartennummer** funktioniert?</span><span class="sxs-lookup"><span data-stu-id="ab515-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ab515-111">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn Sie ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="ab515-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="ab515-112">Für eine **Kreditkarten Richtlinie** , die mit einer Konfidenz Stufe von 85% konfiguriert ist, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="ab515-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ab515-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddddddddddddddd) sein können und den Luhn-Test bestehen müssen.</span><span class="sxs-lookup"><span data-stu-id="ab515-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="ab515-114">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplexes und robustes Muster, das Karten von allen wichtigen Marken weltweit erkennt, einschließlich Visa, Mastercard, Discover Card, JCB, American Express, Geschenkkarten und Diner Cards.</span><span class="sxs-lookup"><span data-stu-id="ab515-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="ab515-115">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Luhn-Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="ab515-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="ab515-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="ab515-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ab515-117">Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="ab515-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ab515-118">Eine der folgenden Bedingungen trifft zu:</span><span class="sxs-lookup"><span data-stu-id="ab515-118">One of the following is true:</span></span>

  - <span data-ttu-id="ab515-119">Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="ab515-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="ab515-120">Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="ab515-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="ab515-121">Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.</span><span class="sxs-lookup"><span data-stu-id="ab515-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="ab515-122">Die Prüfsummen Übergabe</span><span class="sxs-lookup"><span data-stu-id="ab515-122">The checksum passes</span></span>

    <span data-ttu-id="ab515-123">Beispielsweise würde das folgende Beispiel für eine DLP-Kreditkartennummern Richtlinie ausgelöst werden:</span><span class="sxs-lookup"><span data-stu-id="ab515-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="ab515-124">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="ab515-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="ab515-125">Gültig bis: 2/2009</span><span class="sxs-lookup"><span data-stu-id="ab515-125">Expires: 2/2009</span></span>

<span data-ttu-id="ab515-126">Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für Kreditkarte suchen #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="ab515-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="ab515-127">Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ab515-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  