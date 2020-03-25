---
title: DLP-Regel für US/UK-Passport-Nummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931261"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="ea7f9-102">Probleme mit DLP-US/UK-Passport-Nummern</span><span class="sxs-lookup"><span data-stu-id="ea7f9-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="ea7f9-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ea7f9-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ea7f9-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ea7f9-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ea7f9-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ea7f9-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ea7f9-109">**DLP-Probleme mit US/UK-Passport-Nummern**</span><span class="sxs-lookup"><span data-stu-id="ea7f9-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="ea7f9-110">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei der Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **US/UK-Passport-Nummer** funktioniert?</span><span class="sxs-lookup"><span data-stu-id="ea7f9-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ea7f9-111">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dafür enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="ea7f9-112">Für eine **US/UK-Passport-Nummern** Richtlinie, die mit einer Konfidenz Stufe von 75% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="ea7f9-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neun Ziffern</span><span class="sxs-lookup"><span data-stu-id="ea7f9-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="ea7f9-114">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neun aufeinanderfolgende Ziffern</span><span class="sxs-lookup"><span data-stu-id="ea7f9-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="ea7f9-115">**[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, es gibt keine Prüfsumme</span><span class="sxs-lookup"><span data-stu-id="ea7f9-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="ea7f9-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Eine DLP-Richtlinie ist 75% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="ea7f9-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ea7f9-117">Die Funktion Func_usa_uk_passport findet Inhalte, die dem Muster entsprechen.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ea7f9-118">Ein Schlüsselwort aus Keyword_passport wurde gefunden.</span><span class="sxs-lookup"><span data-stu-id="ea7f9-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="ea7f9-119">Das folgende Beispiel würde beispielsweise für die **US/UK-Passport-Nummern** Richtlinie ausgelöst: U.S. Passport-Nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="ea7f9-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="ea7f9-120">Weitere Informationen dazu, was erforderlich ist, damit eine US/UK-Passport-Nummer für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [welche Arten von vertraulichen Informationen suchen nach US/UK Passport-Nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="ea7f9-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="ea7f9-121">Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ea7f9-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  