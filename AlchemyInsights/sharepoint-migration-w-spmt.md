---
title: SharePoint-Migration mit SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931549"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="6270c-102">SharePoint-Migration mit SPMT</span><span class="sxs-lookup"><span data-stu-id="6270c-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="6270c-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="6270c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6270c-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="6270c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6270c-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="6270c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6270c-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="6270c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6270c-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="6270c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6270c-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="6270c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6270c-109">**SharePoint-Migrationstool**</span><span class="sxs-lookup"><span data-stu-id="6270c-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="6270c-110">Mit dem SharePoint-Migrations Tool können Sie Ihre Daten in die Cloud übertragen und die neueste Zusammenarbeit, die neuesten Informationen und die neuen Funktionen nutzen, um Sie für Migrationen von den kleinsten Dateigruppen bis hin zu einer großen Unternehmens Migration zu verwenden. Sicherheitslösungen mit Office 365.</span><span class="sxs-lookup"><span data-stu-id="6270c-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="6270c-111">Herunterladen und Installieren des SharePoint-Migrationstools</span><span class="sxs-lookup"><span data-stu-id="6270c-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="6270c-112">Problembehandlung häufig auftretender SPMT-Probleme und Fehler</span><span class="sxs-lookup"><span data-stu-id="6270c-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="6270c-113">Behandlung von SPMT-Installationsproblemen</span><span class="sxs-lookup"><span data-stu-id="6270c-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
