---
title: Verzögerungen beim Empfang von SharePoint-und OneDrive-Warnungen
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771214"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="33758-102">Verzögerungen beim Empfang von SharePoint-und OneDrive-Warnungen</span><span class="sxs-lookup"><span data-stu-id="33758-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="33758-103">Überprüfen Sie zuerst den Junk-oder Spam-Ordner in Ihrer e-Mail.</span><span class="sxs-lookup"><span data-stu-id="33758-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="33758-104">Wenn **sich alle Warnungen aus mehreren Dateien oder Bibliotheken verzögert**haben, besuchen Sie das [Service-Integritäts Dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) , um nach eventuellen Ankündigungen/Vorfällen zu suchen, die mit SharePoint oder Exchange möglicherweise auftreten.</span><span class="sxs-lookup"><span data-stu-id="33758-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="33758-105">Das Problem kann mit der SharePoint-Benachrichtigungsfunktion oder mit Verzögerungen bei e-Mails über Exchange auftreten.</span><span class="sxs-lookup"><span data-stu-id="33758-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="33758-106">Beachten Sie auch, ob andere e-Mails zugestellt werden – wenn nicht, liegt das Problem wahrscheinlich bei Exchange-Verzögerungen.</span><span class="sxs-lookup"><span data-stu-id="33758-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="33758-107">Wenn **eine einzelne Warnung aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird**, versuchen Sie, Sie zu löschen und neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="33758-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="33758-108">Informationen zum erneuten Erstellen der Benachrichtigung finden Sie unter [verwalten, anzeigen oder Löschen von SharePoint-Warnungen](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="33758-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="33758-109">Benachrichtigungen können nicht an eine Verteilergruppe gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="33758-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="33758-110">Es werden nur Sicherheits-und O365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33758-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="33758-111">Sie können keine e-Mail-Benachrichtigungsvorlagen anpassen.</span><span class="sxs-lookup"><span data-stu-id="33758-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="33758-112">Sie müssen Microsoft Flow oder SharePoint Designer Workflow verwenden, um diese zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="33758-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
