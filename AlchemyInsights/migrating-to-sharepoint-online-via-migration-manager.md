---
title: Migrieren zu SharePoint Online über den Migrations-Manager
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931975"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="43cb3-102">Migrieren zu SharePoint Online über den Migrations-Manager</span><span class="sxs-lookup"><span data-stu-id="43cb3-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="43cb3-103">**Wichtig**: Viele SharePoint Online- und OneDrive-Kunden führen im Hintergrund geschäftskritische Anwendungen für den Dienst aus.</span><span class="sxs-lookup"><span data-stu-id="43cb3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="43cb3-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="43cb3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="43cb3-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="43cb3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="43cb3-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="43cb3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="43cb3-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="43cb3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="43cb3-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="43cb3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="43cb3-109">**Migrations-Manager**</span><span class="sxs-lookup"><span data-stu-id="43cb3-109">**Migration Manager**</span></span>

<span data-ttu-id="43cb3-110">Der Migrations-Manager befindet sich im modernen SharePoint Admin Center und führt Sie durch die Einrichtung Ihrer Clients und das Erstellen von Aufgaben.</span><span class="sxs-lookup"><span data-stu-id="43cb3-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="43cb3-111">Sie können globale oder aufgabenbezogene Einstellungen festlegen, den aggregierten Status des gesamten Vorgangs anzeigen sowie Zusammenfassungs- und aufgabenbezogene Berichte herunterladen.</span><span class="sxs-lookup"><span data-stu-id="43cb3-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="43cb3-112">Erste Schritte mit dem Migrations-Manager</span><span class="sxs-lookup"><span data-stu-id="43cb3-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="43cb3-113">Einrichten der Migrations-Manager-Clients</span><span class="sxs-lookup"><span data-stu-id="43cb3-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="43cb3-114">Einstellungen des Migrations-Managers</span><span class="sxs-lookup"><span data-stu-id="43cb3-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
