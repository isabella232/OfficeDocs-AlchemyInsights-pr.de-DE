---
title: Problembehandlung von Problemen und Fehlern beim SharePoint-Migrations Tool
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931117"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="c2179-102">Problembehandlung von Problemen und Fehlern beim SharePoint-Migrations Tool</span><span class="sxs-lookup"><span data-stu-id="c2179-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="c2179-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c2179-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c2179-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="c2179-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c2179-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="c2179-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c2179-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="c2179-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c2179-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="c2179-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c2179-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="c2179-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c2179-109">**Häufige Probleme und Fehler**</span><span class="sxs-lookup"><span data-stu-id="c2179-109">**Common issues and errors**</span></span>

<span data-ttu-id="c2179-110">Bei der Verwendung des SharePoint-Migrationstools (SPMT) treten möglicherweise einige häufig auftretende Probleme auf.</span><span class="sxs-lookup"><span data-stu-id="c2179-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="c2179-111">Weitere Informationen finden Sie unter den Links unten.</span><span class="sxs-lookup"><span data-stu-id="c2179-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="c2179-112">Problembehandlung häufig auftretender SPMT-Probleme und Fehler</span><span class="sxs-lookup"><span data-stu-id="c2179-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="c2179-113">Problembehandlung bei SPMT-Installationsproblemen</span><span class="sxs-lookup"><span data-stu-id="c2179-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)