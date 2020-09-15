---
title: DLP-Regel für US-Bank Kontonummer nicht funktionsfähig
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679295"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="ece4f-102">DLP-Probleme mit US-Bank Kontonummern</span><span class="sxs-lookup"><span data-stu-id="ece4f-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="ece4f-103">**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="ece4f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ece4f-104">**DLP-Probleme mit US-Bank Kontonummern**</span><span class="sxs-lookup"><span data-stu-id="ece4f-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="ece4f-105">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **US-Bank Kontonummer** funktioniert?</span><span class="sxs-lookup"><span data-stu-id="ece4f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ece4f-106">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dafür enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="ece4f-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="ece4f-107">Für eine **US-Bank Kontonummern** Richtlinie, die mit einer Konfidenz Stufe von 85% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:</span><span class="sxs-lookup"><span data-stu-id="ece4f-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ece4f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 Ziffern</span><span class="sxs-lookup"><span data-stu-id="ece4f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="ece4f-109">**[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 aufeinanderfolgende Ziffern.</span><span class="sxs-lookup"><span data-stu-id="ece4f-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="ece4f-110">**[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nein, es gibt keine Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="ece4f-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="ece4f-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Eine DLP-Richtlinie ist 75% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="ece4f-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ece4f-112">Der reguläre Ausdruck Regex_usa_bank_account_number findet Inhalte, die mit dem Muster übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="ece4f-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="ece4f-113">Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="ece4f-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="ece4f-114">Das folgende Beispiel würde beispielsweise für die US- **Bank Kontonummern** Richtlinie ausgelöst: Girokonto 78344011</span><span class="sxs-lookup"><span data-stu-id="ece4f-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="ece4f-115">Weitere Informationen darüber, was erforderlich ist, damit eine **US-Bank Kontonummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für die US-Bankkontonummer suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="ece4f-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="ece4f-116">Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="ece4f-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  