---
title: SharePoint-Migrationsleistung
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932003"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="4eaf9-102">SharePoint-Migrationsleistung</span><span class="sxs-lookup"><span data-stu-id="4eaf9-102">SharePoint migration performance</span></span>

<span data-ttu-id="4eaf9-103">**Wichtig**: Viele SharePoint Online- und OneDrive-Kunden führen im Hintergrund geschäftskritische Anwendungen für den Dienst aus.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4eaf9-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4eaf9-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4eaf9-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4eaf9-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4eaf9-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4eaf9-109">**Migrationsleistung**</span><span class="sxs-lookup"><span data-stu-id="4eaf9-109">**Migration performance**</span></span>

<span data-ttu-id="4eaf9-p103">Die Migrationsleistung kann durch die Netzwerkinfrastruktur, Dateigröße, Migrationszeit und Drosselung beeinträchtigt werden. Das Verständnis dieser Faktoren hilft Ihnen dabei, Ihre Migration zu planen und die Effizienz zu maximieren.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="4eaf9-112">Besuchen Sie die untenstehenden Links, um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="4eaf9-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="4eaf9-113">SharePoint Online und ODB-Migrationsgeschwindigkeit</span><span class="sxs-lookup"><span data-stu-id="4eaf9-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="4eaf9-114">Vermeiden von Einschränkungen oder Sperren in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4eaf9-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="4eaf9-115">Herunterladen und Installieren des SharePoint-Migrationstools</span><span class="sxs-lookup"><span data-stu-id="4eaf9-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
