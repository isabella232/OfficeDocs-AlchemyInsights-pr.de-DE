---
title: SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36744640"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="311ee-102">SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt</span><span class="sxs-lookup"><span data-stu-id="311ee-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="311ee-103">Überprüfen Sie den Ordner Junk in Ihrer e-Mail, da manchmal Warnungen möglicherweise dorthin gelangen.</span><span class="sxs-lookup"><span data-stu-id="311ee-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="311ee-104">Ermitteln Sie, ob **alle Warnungen nicht zugestellt werden** oder ob **eine einzelne Warnung** aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird.</span><span class="sxs-lookup"><span data-stu-id="311ee-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="311ee-105">**Einzelne Warnungen werden nicht zugestellt**: Wenn eine einzelne Warnung aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird, können Sie versuchen, Sie zu löschen und neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="311ee-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="311ee-106">Informationen zum erneuten Erstellen der Benachrichtigung finden Sie unter [verwalten, anzeigen oder Löschen von SharePoint-Warnungen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) .</span><span class="sxs-lookup"><span data-stu-id="311ee-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="311ee-107">**Alle Warnungen werden nicht zugestellt**: Wenn alle Warnungen aus mehreren Dateien oder Bibliotheken nicht zugestellt werden, besuchen Sie das [Service-Integritäts Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , um nach eventuellen Ratschlägen/Vorfällen zu suchen, die mit SharePoint oder Exchange möglicherweise auftreten.</span><span class="sxs-lookup"><span data-stu-id="311ee-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="311ee-108">Das Problem kann mit der SharePoint-Benachrichtigungsfunktion oder mit Verzögerungen in e-Mails durch Exchange auftreten.</span><span class="sxs-lookup"><span data-stu-id="311ee-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="311ee-109">Es wird auch wichtig sein zu beachten, ob andere e-Mails zugestellt werden, und wenn nicht, ist das Problem wahrscheinlich bei Exchange-Verzögerungen.</span><span class="sxs-lookup"><span data-stu-id="311ee-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="311ee-110">FAQ für Benachrichtigungen:</span><span class="sxs-lookup"><span data-stu-id="311ee-110">FAQ on alerts:</span></span>

- <span data-ttu-id="311ee-111">Es ist nicht möglich, Warnungen an die Verteilergruppe zu senden, sondern nur Sicherheits-und O365-Gruppen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="311ee-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="311ee-112">Sie können keine e-Mail-Benachrichtigungsvorlagen anpassen. Sie müssen Microsoft Flow oder SharePoint Designer Workflow verwenden, um diese zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="311ee-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="311ee-113">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="311ee-113">More Information:</span></span>

- <span data-ttu-id="311ee-114">**Warnungs Setup**: Weitere Informationen zum Einrichten von Warnungen finden Sie unter [Erstellen einer Warnung, um benachrichtigt zu werden, wenn sich eine Datei oder ein Ordner in SharePoint ändert](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="311ee-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="311ee-115">**Problembehandlung bei Warnungen**: Weitere Informationen zur Problembehandlung bei Warnungen finden Sie unter [Benutzer erhalten keine SharePoint Online Benachrichtigungs Benachrichtigungen](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="311ee-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="311ee-116">**Richtlinien für erweiterte O365-Konformitäts**Warnungen: Weitere Informationen zum Einrichten dieser Warnungen finden Sie unter [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="311ee-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="311ee-117">**SharePoint-und OneDrive-Überwachungsprotokolle**: Weitere Informationen zum Abrufen dieser Ereignisse finden Sie unter [Durchsuchen des Überwachungsprotokolls](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="311ee-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="311ee-118">**Von Advanced Threat Protection gesendete Warnungen**: siehe [ATP für SharePoint und OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="311ee-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="311ee-119">**Von Data Loss Prevention Policies gesendete Warnungen**: siehe [e-Mail-Benachrichtigungen für DLP-Richtlinien](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="311ee-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="311ee-120">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="311ee-120">Related Topics</span></span>

<span data-ttu-id="311ee-121">Möchten Sie Microsoft Flow in SharePoint Online testen?</span><span class="sxs-lookup"><span data-stu-id="311ee-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="311ee-122">Fluss erstellen</span><span class="sxs-lookup"><span data-stu-id="311ee-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="311ee-123">SharePoint und Flow</span><span class="sxs-lookup"><span data-stu-id="311ee-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
