---
title: Weitere Informationen zu DLP-Problemen
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932693"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="7e72c-102">Informationen zu DLP-Problemen</span><span class="sxs-lookup"><span data-stu-id="7e72c-102">Information about DLP issues</span></span>

<span data-ttu-id="7e72c-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="7e72c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7e72c-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="7e72c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7e72c-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="7e72c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7e72c-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="7e72c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7e72c-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="7e72c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7e72c-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="7e72c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7e72c-109">**Informationen zur DLP-Richtlinie**</span><span class="sxs-lookup"><span data-stu-id="7e72c-109">**Information on DLP policy**</span></span>

<span data-ttu-id="7e72c-110">Mit einer DLP-Richtlinie können Sie vertrauliche Informationen über Office 365 identifizieren, überwachen und automatisch schützen.</span><span class="sxs-lookup"><span data-stu-id="7e72c-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="7e72c-111">Weitere Informationen finden Sie unter den folgenden Links:</span><span class="sxs-lookup"><span data-stu-id="7e72c-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="7e72c-112">Verhinderung von Datenverlust – Übersicht</span><span class="sxs-lookup"><span data-stu-id="7e72c-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="7e72c-113">Wonach die Typen von vertraulichen Informationen suchen</span><span class="sxs-lookup"><span data-stu-id="7e72c-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="7e72c-114">Erstellen eines benutzerdefinierten vertraulichen Informationstyps</span><span class="sxs-lookup"><span data-stu-id="7e72c-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="7e72c-115">Senden von e-Mail-Benachrichtigungen und Anzeigen von Richtlinien Tipps</span><span class="sxs-lookup"><span data-stu-id="7e72c-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="7e72c-116">Protect SharePoint Online files with retention labels and DLP</span><span class="sxs-lookup"><span data-stu-id="7e72c-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="7e72c-117">DLP und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7e72c-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="7e72c-118">Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten Typ vertraulicher Informationen testen möchten, verwenden Sie die Option **Testtyp** unter **Klassifikationen** > **vertrauliche Informationstypen**.</span><span class="sxs-lookup"><span data-stu-id="7e72c-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="7e72c-119">Weitere Informationen finden Sie unter [Testen benutzerdefinierter vertraulicher Informationstypen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="7e72c-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>