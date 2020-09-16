---
title: SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751242"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="b87e8-102">SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt</span><span class="sxs-lookup"><span data-stu-id="b87e8-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="b87e8-103">Überprüfen Sie den Ordner Junk in Ihrer e-Mail, da manchmal Warnungen möglicherweise dorthin gelangen.</span><span class="sxs-lookup"><span data-stu-id="b87e8-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="b87e8-104">Ermitteln Sie, ob **alle Warnungen nicht zugestellt werden** oder ob **eine einzelne Warnung** aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird.</span><span class="sxs-lookup"><span data-stu-id="b87e8-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="b87e8-105">**Einzelne Warnungen werden nicht zugestellt**: Wenn eine einzelne Warnung aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird, können Sie versuchen, Sie zu löschen und neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="b87e8-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="b87e8-106">Informationen zum erneuten Erstellen der Benachrichtigung finden Sie unter [verwalten, anzeigen oder Löschen von SharePoint-Warnungen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="b87e8-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="b87e8-107">**Alle Warnungen werden nicht zugestellt**: Wenn alle Warnungen aus mehreren Dateien oder Bibliotheken nicht zugestellt werden, besuchen Sie das [Service-Integritäts Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , um nach eventuellen Ratschlägen/Vorfällen zu suchen, die mit SharePoint oder Exchange möglicherweise auftreten.</span><span class="sxs-lookup"><span data-stu-id="b87e8-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="b87e8-108">Das Problem kann mit der SharePoint-Benachrichtigungsfunktion oder mit Verzögerungen in e-Mails durch Exchange auftreten.</span><span class="sxs-lookup"><span data-stu-id="b87e8-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="b87e8-109">Es wird auch wichtig sein zu beachten, ob andere e-Mails zugestellt werden, und wenn nicht, ist das Problem wahrscheinlich bei Exchange-Verzögerungen.</span><span class="sxs-lookup"><span data-stu-id="b87e8-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="b87e8-110">FAQ für Benachrichtigungen:</span><span class="sxs-lookup"><span data-stu-id="b87e8-110">FAQ on alerts:</span></span>

- <span data-ttu-id="b87e8-111">Es ist nicht möglich, Warnungen an die Verteilergruppe zu senden, sondern nur Sicherheits-und O365-Gruppen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b87e8-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="b87e8-112">Sie können keine e-Mail-Benachrichtigungsvorlagen anpassen. Sie müssen Microsoft Flow oder SharePoint Designer Workflow verwenden, um diese zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="b87e8-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="b87e8-113">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="b87e8-113">Related Topics</span></span>

<span data-ttu-id="b87e8-114">Möchten Sie Microsoft Flow in SharePoint Online testen?</span><span class="sxs-lookup"><span data-stu-id="b87e8-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="b87e8-115">Fluss erstellen</span><span class="sxs-lookup"><span data-stu-id="b87e8-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="b87e8-116">SharePoint und Flow</span><span class="sxs-lookup"><span data-stu-id="b87e8-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
