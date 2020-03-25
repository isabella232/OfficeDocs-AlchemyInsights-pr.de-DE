---
title: DLP-Richtlinien Tipps funktionieren nicht
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932585"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="0126c-102">Probleme mit dem DLP-richtlinientipp</span><span class="sxs-lookup"><span data-stu-id="0126c-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="0126c-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="0126c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0126c-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="0126c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0126c-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="0126c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0126c-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="0126c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0126c-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="0126c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0126c-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="0126c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0126c-109">**DLP-Richtlinien Tipps**</span><span class="sxs-lookup"><span data-stu-id="0126c-109">**DLP policy tips**</span></span>

<span data-ttu-id="0126c-110">Bei der Verwendung von **DLP-Richtlinien**können Benutzer über eine Richtlinienverletzung mit **Richtlinien Tipps**informiert werden.</span><span class="sxs-lookup"><span data-stu-id="0126c-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="0126c-111">Administratoren können Richtlinien Tipps so konfigurieren, dass Sie beim Testen Ihrer DLP-Richtlinie angezeigt werden oder wenn sich die Richtlinie im vollständigen Erzwingungsmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="0126c-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="0126c-112">Gehen Sie folgendermaßen vor, um Richtlinien Tipps für ihre DLP-Richtlinie im Security and Compliance Center im vollständigen Durchsetzungs Modus zu konfigurieren:</span><span class="sxs-lookup"><span data-stu-id="0126c-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="0126c-113">Stellen Sie sicher, dass in der DLP-Regel mithilfe der [hier](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)beschriebenen Schritte Richtlinien Tipps **aktiviert** wurden.</span><span class="sxs-lookup"><span data-stu-id="0126c-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="0126c-114">Stellen Sie sicher, dass Ihre Inhalte [hier](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) **übereinstimmen** , die **erforderlich** sind, um die in diesem Artikel dargelegte Regel auszulösen.</span><span class="sxs-lookup"><span data-stu-id="0126c-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="0126c-115">Richtlinien Tipps werden sowohl in OWA als auch in Outlook angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0126c-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="0126c-116">Wenn Sie jedoch **Outlook 2013 oder höher**verwenden, werden Richtlinien Tipps nur unter bestimmten Bedingungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0126c-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="0126c-117">Diese Bedingungen sind hier aufgelistet: [unterstützte Bedingungen für Outlook 2013 oder höher zum Anzeigen von Richtlinien Tipps](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="0126c-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="0126c-118">Weitere Informationen zu DLP-Richtlinien Tipps finden Sie unter: [Anzeigen von Richtlinien Tipps für DLP-Richtlinien](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="0126c-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  