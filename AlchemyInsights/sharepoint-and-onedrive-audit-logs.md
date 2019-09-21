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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068022"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="8ba5f-102">SharePoint-und OneDrive-Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="8ba5f-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="8ba5f-103">**Moderne Unified Audit-Protokolle von SharePoint und OneDrive aus Compliance**</span><span class="sxs-lookup"><span data-stu-id="8ba5f-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="8ba5f-104">Aktivieren/Deaktivieren der einheitlichen Überwachungsprotokollierung</span><span class="sxs-lookup"><span data-stu-id="8ba5f-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="8ba5f-105">In SharePoint oder OneDrive ist keine zusätzliche Konfiguration erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="8ba5f-106">Verwenden Sie die Überwachungs Protokollierungs Suche, um die Aktivität der Datei (en), des Ordners (s), des (der) Benutzers (s), der Berechtigungen zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="8ba5f-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="8ba5f-107">Datei-und Seiten Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="8ba5f-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="8ba5f-108">Ordner Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="8ba5f-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="8ba5f-109">Freigabe-und Zugriffs Anforderungs Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="8ba5f-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="8ba5f-110">Synchronisierungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="8ba5f-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="8ba5f-111">Website Verwaltungsaktivitäten</span><span class="sxs-lookup"><span data-stu-id="8ba5f-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="8ba5f-112">Weitere Informationen zum Abrufen dieser Ereignisse finden Sie unter [Durchsuchen des Überwachungsprotokolls](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="8ba5f-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="8ba5f-113">**Klassische SharePoint-Überwachungsprotokolle**</span><span class="sxs-lookup"><span data-stu-id="8ba5f-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="8ba5f-114">Wir haben die SPO-Legacy Überwachung in ein einheitliches Überwachungsprotokoll migriert.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="8ba5f-115">Dies bedeutet im Wesentlichen, dass alle SPO-Legacy-Überwachungsberichte jetzt über unterstützt werden, und die Legacy-Überwachungssignale wurden zu "ausgehend" migriert.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="8ba5f-116">Wichtige Änderungen:</span><span class="sxs-lookup"><span data-stu-id="8ba5f-116">Key changes:</span></span>

- <span data-ttu-id="8ba5f-117">Das kürzen als Funktion ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="8ba5f-118">Der Abschnitt, in dem Sie bestimmte zu überwachende Ereignisse auswählen, ist nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="8ba5f-119">In [diesem Dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) finden Sie eine vollständige Liste überwachter Ereignisse, die standardmäßig verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="8ba5f-120">Die Option "Standort" unter **angepasste Berichte** steht nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="8ba5f-121">Ereignisse für das Öffnen oder Herunterladen von Dokumenten stehen nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-121">“Opening or downloading documents” events is NOT available.</span></span> 

