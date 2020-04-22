---
title: Klassische SharePoint-Überwachungsprotokollberichte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741964"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="ad71f-102">SharePoint-und OneDrive-Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="ad71f-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="ad71f-103">Klassische SharePoint-Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="ad71f-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="ad71f-104">Die SPO-Legacy Überwachung wurde zu einem einheitlichen Überwachungsprotokoll migriert.</span><span class="sxs-lookup"><span data-stu-id="ad71f-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="ad71f-105">Alle SPO-Legacy-Überwachungsberichte werden nun über unterstützt, und die Legacy-Überwachungssignale wurden zu "ausgehend" migriert.</span><span class="sxs-lookup"><span data-stu-id="ad71f-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="ad71f-106">Wichtige Änderungen:</span><span class="sxs-lookup"><span data-stu-id="ad71f-106">Key changes:</span></span>

* <span data-ttu-id="ad71f-107">Trimmen ist nicht als Funktion verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ad71f-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="ad71f-108">Das Auswählen bestimmter zu überwachenden Ereignisse ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ad71f-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="ad71f-109">In [diesem Dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) finden Sie eine vollständige Liste überwachter Ereignisse, die standardmäßig verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="ad71f-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="ad71f-110">Die Option **Speicherort** unter **angepasste Berichte** ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ad71f-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="ad71f-111">Die Option zum **Öffnen oder Herunterladen von Dokument** Ereignissen ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ad71f-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="ad71f-112">Konfigurieren von Überwachungseinstellungen für eine Websitesammlung</span><span class="sxs-lookup"><span data-stu-id="ad71f-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="ad71f-113">Moderne Unified Audit-Protokolle von SharePoint und OneDrive aus Compliance</span><span class="sxs-lookup"><span data-stu-id="ad71f-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="ad71f-114">Aktivieren/Deaktivieren der einheitlichen Überwachungsprotokollierung</span><span class="sxs-lookup"><span data-stu-id="ad71f-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="ad71f-115">In SharePoint oder OneDrive ist keine zusätzliche Konfiguration erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad71f-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="ad71f-116">Verwenden Sie die Überwachungs Protokollierungs Suche, um die Aktivität der Datei (en), des Ordners (s), des (der) Benutzers (s), der Berechtigungen zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="ad71f-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="ad71f-117">Datei- und Seitenaktivitäten</span><span class="sxs-lookup"><span data-stu-id="ad71f-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="ad71f-118">Ordneraktivitäten</span><span class="sxs-lookup"><span data-stu-id="ad71f-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="ad71f-119">Freigabe- und Zugriffsanforderungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="ad71f-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="ad71f-120">Synchronisierungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="ad71f-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="ad71f-121">Websiteverwaltungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="ad71f-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="ad71f-122">Weitere Informationen zum Abrufen dieser Ereignisse finden Sie unter [Durchsuchen des Überwachungsprotokolls](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ad71f-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
