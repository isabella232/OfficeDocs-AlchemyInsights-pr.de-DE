---
title: Migrieren von Optionen zu SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932729"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="2660e-102">Migrieren von Optionen zu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2660e-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="2660e-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2660e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2660e-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="2660e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2660e-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="2660e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2660e-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="2660e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2660e-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="2660e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2660e-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="2660e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2660e-109">**Migrationsoptionen**</span><span class="sxs-lookup"><span data-stu-id="2660e-109">**Migration options**</span></span>

<span data-ttu-id="2660e-110">Es stehen verschiedene Optionen zur Verfügung, um Inhalte in SharePoint Online zu migrieren, je nach Größe und Menge der Dateien, die Sie verschieben müssen, finden Sie eine Liste der Optionen, die [sich hier befinden](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="2660e-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="2660e-111">Weitere Informationen zur Inhaltsmigration finden Sie unter den Links unten.</span><span class="sxs-lookup"><span data-stu-id="2660e-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="2660e-112">SharePoint-Migrations Tool</span><span class="sxs-lookup"><span data-stu-id="2660e-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="2660e-113">Erste Schritte mit dem Migrations-Manager</span><span class="sxs-lookup"><span data-stu-id="2660e-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="2660e-114">SharePoint Online-und ODB-Migrations Geschwindigkeit</span><span class="sxs-lookup"><span data-stu-id="2660e-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="2660e-115">Vermeiden von Einschränkungen oder Sperren in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2660e-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="2660e-116">SharePoint Migration Assessment Tool (smat)</span><span class="sxs-lookup"><span data-stu-id="2660e-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="2660e-117">**Hinweis**: das SharePoint-Migrationstool unterstützt derzeit nur Migrationen von SharePoint 2010 und 2013.</span><span class="sxs-lookup"><span data-stu-id="2660e-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="2660e-118">Version 2016 oder 2019 werden zu diesem Zeitpunkt nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2660e-118">Version 2016 or 2019 are not supported at this time.</span></span>
