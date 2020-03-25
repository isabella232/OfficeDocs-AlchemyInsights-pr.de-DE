---
title: DLP-Regel für US-Bank Kontonummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932532"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="a5ded-102">DLP-Probleme mit US-Bank Kontonummern</span><span class="sxs-lookup"><span data-stu-id="a5ded-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="a5ded-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="a5ded-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a5ded-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="a5ded-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a5ded-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="a5ded-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a5ded-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="a5ded-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a5ded-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="a5ded-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a5ded-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="a5ded-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a5ded-109">**DLP-Probleme mit US-Bank Kontonummern**</span><span class="sxs-lookup"><span data-stu-id="a5ded-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="a5ded-110">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **US-Bank Kontonummer** funktioniert?</span><span class="sxs-lookup"><span data-stu-id="a5ded-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a5ded-111">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dafür enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="a5ded-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a5ded-112">Für eine **US-Bank Kontonummern** Richtlinie, die mit einer Konfidenz Stufe von 85% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="a5ded-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a5ded-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 Ziffern</span><span class="sxs-lookup"><span data-stu-id="a5ded-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="a5ded-114">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 aufeinanderfolgende Ziffern.</span><span class="sxs-lookup"><span data-stu-id="a5ded-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="a5ded-115">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, es gibt keine Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="a5ded-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a5ded-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Eine DLP-Richtlinie ist 75% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="a5ded-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a5ded-117">Der reguläre Ausdruck Regex_usa_bank_account_number findet Inhalte, die mit dem Muster übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="a5ded-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="a5ded-118">Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="a5ded-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="a5ded-119">Das folgende Beispiel würde beispielsweise für die US- **Bank Kontonummern** Richtlinie ausgelöst: Girokonto 78344011</span><span class="sxs-lookup"><span data-stu-id="a5ded-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="a5ded-120">Weitere Informationen darüber, was erforderlich ist, damit eine **US-Bank Kontonummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für die US-Bankkontonummer suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="a5ded-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="a5ded-121">Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a5ded-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  