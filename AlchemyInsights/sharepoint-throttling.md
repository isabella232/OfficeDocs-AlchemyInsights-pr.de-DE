---
title: SharePoint Online Drosselung
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931441"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="f4807-102">SharePoint Online Drosselung</span><span class="sxs-lookup"><span data-stu-id="f4807-102">SharePoint Online throttling</span></span>

<span data-ttu-id="f4807-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f4807-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f4807-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="f4807-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f4807-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="f4807-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f4807-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="f4807-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f4807-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="f4807-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f4807-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="f4807-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f4807-109">**SharePoint Online Drosselung**</span><span class="sxs-lookup"><span data-stu-id="f4807-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="f4807-110">SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten.</span><span class="sxs-lookup"><span data-stu-id="f4807-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="f4807-111">Einschränkungsgrenzwerte Ruft die Anzahl von Aktionen eines Benutzers oder gleichzeitige (von Code- oder Skriptblock), um Ressourcen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="f4807-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="f4807-112">Weitere Informationen finden Sie unter den Links unten.</span><span class="sxs-lookup"><span data-stu-id="f4807-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="f4807-113">Vermeiden von Einschränkungen oder Sperren in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f4807-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="f4807-114">Daten Migration und SPO-Drosselung</span><span class="sxs-lookup"><span data-stu-id="f4807-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="f4807-115">SharePoint Online und OneDrive-Migrationsgeschwindigkeit</span><span class="sxs-lookup"><span data-stu-id="f4807-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="f4807-116">Behandeln von Einschränkungen in SharePoint Online mit exponentiellem Backoff</span><span class="sxs-lookup"><span data-stu-id="f4807-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="f4807-117">Kapazitätsplanung und Auslastungstests für SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f4807-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

