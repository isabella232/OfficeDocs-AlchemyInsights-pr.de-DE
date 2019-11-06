---
title: Klassische SharePoint-Überwachungsprotokollberichte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992617"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="a09db-102">SharePoint-und OneDrive-Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="a09db-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="a09db-103">Klassische SharePoint-Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="a09db-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="a09db-104">Die SPO-Legacy Überwachung wurde zu einem einheitlichen Überwachungsprotokoll migriert.</span><span class="sxs-lookup"><span data-stu-id="a09db-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="a09db-105">Alle SPO-Legacy-Überwachungsberichte werden nun über unterstützt, und die Legacy-Überwachungssignale wurden zu "ausgehend" migriert.</span><span class="sxs-lookup"><span data-stu-id="a09db-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="a09db-106">Wichtige Änderungen:</span><span class="sxs-lookup"><span data-stu-id="a09db-106">Key changes:</span></span>

* <span data-ttu-id="a09db-107">Trimmen ist nicht als Funktion verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a09db-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="a09db-108">Das Auswählen bestimmter zu überwachenden Ereignisse ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a09db-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="a09db-109">In [diesem Dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) finden Sie eine vollständige Liste überwachter Ereignisse, die standardmäßig verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="a09db-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="a09db-110">Die Option **Speicherort** unter **angepasste Berichte** ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a09db-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="a09db-111">Die Option zum **Öffnen oder Herunterladen von Dokument** Ereignissen ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a09db-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="a09db-112">Konfigurieren von Überwachungseinstellungen für eine Websitesammlung</span><span class="sxs-lookup"><span data-stu-id="a09db-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="a09db-113">Moderne Unified Audit-Protokolle von SharePoint und OneDrive aus Compliance</span><span class="sxs-lookup"><span data-stu-id="a09db-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="a09db-114">Aktivieren/Deaktivieren der einheitlichen Überwachungsprotokollierung</span><span class="sxs-lookup"><span data-stu-id="a09db-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="a09db-115">In SharePoint oder OneDrive ist keine zusätzliche Konfiguration erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a09db-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="a09db-116">Verwenden Sie die Überwachungs Protokollierungs Suche, um die Aktivität der Datei (en), des Ordners (s), des (der) Benutzers (s), der Berechtigungen zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="a09db-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="a09db-117">Datei-und Seiten Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="a09db-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="a09db-118">Ordner Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="a09db-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="a09db-119">Freigabe-und Zugriffs Anforderungs Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="a09db-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="a09db-120">Synchronisierungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="a09db-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="a09db-121">Website Verwaltungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="a09db-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="a09db-122">Weitere Informationen zum Abrufen dieser Ereignisse finden Sie unter [Durchsuchen des Überwachungsprotokolls](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="a09db-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
