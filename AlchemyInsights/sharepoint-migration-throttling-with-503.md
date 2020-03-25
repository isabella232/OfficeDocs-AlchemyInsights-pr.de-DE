---
title: SharePoint-Migrations Einschränkung mit 503 Fehlern
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931657"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="9a5e2-102">SharePoint-Migrations Einschränkung mit 503 Fehlern</span><span class="sxs-lookup"><span data-stu-id="9a5e2-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="9a5e2-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9a5e2-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9a5e2-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9a5e2-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9a5e2-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9a5e2-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9a5e2-109">**503 Fehler beim Migrieren zu SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="9a5e2-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="9a5e2-110">Es wird angezeigt, dass Sie zu SharePoint Online und empfangen von 503-Fehlern migrieren.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="9a5e2-111">Führen Sie die folgenden Schritte aus, damit wir Ihnen so schnell wie möglich behilflich sein können.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="9a5e2-112">Klicken Sie auf **Kontakt Support**und dann auf **Neue Dienstanforderung**.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="9a5e2-113">Geben Sie für den Titel und die Beschreibung **SharePoint-Migrations Einschränkung mit 503**ein.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="9a5e2-114">Sobald das Ticket übermittelt wurde, aktualisieren Sie es mit den folgenden Informationen:</span><span class="sxs-lookup"><span data-stu-id="9a5e2-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="9a5e2-115">Wie viel Links von der Migration (zum Beispiel, wie viele TBS?).</span><span class="sxs-lookup"><span data-stu-id="9a5e2-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="9a5e2-116">Migrations Start-und-Enddatum.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-116">Migration start and end date.</span></span>
    - <span data-ttu-id="9a5e2-117">Beschreiben Sie, wo Sie Ihre Inhalte migrieren, beispielsweise SharePoint Server, Box, GDrive, Dateifreigaben usw.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="9a5e2-118">Schätzen Sie die Anzahl der Einschränkungsfehler (beispielsweise x-Drosselung pro Stunde?) und wann ist die Drosselung aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="9a5e2-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="9a5e2-119">Welches Migrationstool Sie verwenden (beispielsweise SPMT oder ShareGate).</span><span class="sxs-lookup"><span data-stu-id="9a5e2-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


