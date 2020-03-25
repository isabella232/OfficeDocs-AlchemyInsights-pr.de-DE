---
title: Einschränkungen in SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931225"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="21eca-102">Einschränkungen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="21eca-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="21eca-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="21eca-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="21eca-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="21eca-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="21eca-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="21eca-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="21eca-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="21eca-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="21eca-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="21eca-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="21eca-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="21eca-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="21eca-109">**503 Server ist besetzt (Fehler)**</span><span class="sxs-lookup"><span data-stu-id="21eca-109">**503 server is busy error**</span></span>

<span data-ttu-id="21eca-110">Bei dem Versuch, zu SharePoint-oder OneDrive-Websites zu navigieren, erhalten Benutzer möglicherweise einen Fehler "503 Server ist ausgelastet".</span><span class="sxs-lookup"><span data-stu-id="21eca-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="21eca-111">Dieser Fehler kann durch Drosselung im SharePoint-Dienst verursacht werden.</span><span class="sxs-lookup"><span data-stu-id="21eca-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="21eca-112">SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten.</span><span class="sxs-lookup"><span data-stu-id="21eca-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="21eca-113">Einschränkungsgrenzwerte Ruft die Anzahl von Aktionen eines Benutzers oder gleichzeitige (von Code- oder Skriptblock), um Ressourcen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="21eca-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="21eca-114">Weitere Informationen zur Drosselung finden Sie unter vermeiden Sie eine [Drosselung oder Blockierung in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="21eca-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="21eca-115">Wenn Sie der Meinung sind, dass dieser Fehler nicht mit der Einschränkung zusammenhängt, können Sie überprüfen, ob eine aktive Wartung auf Ihrem Mandanten erfolgt, indem Sie zum [Nachrichtencenter](https://portal.office.com/adminportal/home#/MessageCenter)navigieren.</span><span class="sxs-lookup"><span data-stu-id="21eca-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="21eca-116">Vergewissern Sie sich schließlich, dass Sie die Seite [Dienst Integrität](https://portal.office.com/adminportal/home#/servicehealth) besuchen, um nach eventuell auftretenden Warnungen/Vorfällen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="21eca-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

