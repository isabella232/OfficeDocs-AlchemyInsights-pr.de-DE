---
title: Dynamics 365-falsche Dashboard-Shows in Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747639"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="106cb-102">Falsche Dashboard-Anzeige in Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="106cb-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="106cb-103">Es gibt mehrere Gründe, aus denen Sie ein anderes Dashboard als das erwartete anzeigen können:</span><span class="sxs-lookup"><span data-stu-id="106cb-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="106cb-104">Der Benutzer hat ein Standarddashboard für Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="106cb-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="106cb-105">Normalerweise können Sie angeben, dass ein Benutzer Standarddashboard festgelegt wird, wenn die Schaltfläche **als Standard festlegen** in der Befehlsleiste des Dashboards nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="106cb-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="106cb-106">Das Standarddashboard des Benutzers setzt alle anderen Standard Dashboards außer Kraft, auch wenn sich das Standarddashboard des Benutzers nicht in der aktuellen App befindet.</span><span class="sxs-lookup"><span data-stu-id="106cb-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="106cb-107">Verwenden Sie die folgende Problemumgehung, um Ihr Standarddashboard zu löschen.</span><span class="sxs-lookup"><span data-stu-id="106cb-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="106cb-108">Erstellen Sie ein neues persönliches Dashboard.</span><span class="sxs-lookup"><span data-stu-id="106cb-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="106cb-109">Legen Sie das neue Dashboard als Benutzer Standard fest.</span><span class="sxs-lookup"><span data-stu-id="106cb-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="106cb-110">Löschen Sie das Dashboard.</span><span class="sxs-lookup"><span data-stu-id="106cb-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="106cb-111">Das Dashboard wird in der Sitemap festgelegt.</span><span class="sxs-lookup"><span data-stu-id="106cb-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="106cb-112">Sie haben möglicherweise ein Standarddashboard für die Organisation festgelegt, indem Sie ein Dashboard auswählen und "als Standard festlegen" unter "System anpassen" auswählen.</span><span class="sxs-lookup"><span data-stu-id="106cb-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="106cb-113">Das im Sitemap-Designer definierte Dashboard hat jedoch Vorrang vor diesem Dashboard, wenn der Benutzer darauf zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="106cb-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="106cb-114">Um Benutzern das als Organisationsstandard festgelegte Dashboard anzuzeigen, können Sie entweder:</span><span class="sxs-lookup"><span data-stu-id="106cb-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="106cb-115">Festlegen des Dashboards in der Sitemap</span><span class="sxs-lookup"><span data-stu-id="106cb-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="106cb-116">Entfernen des Zugriffs auf das definierte Sitemap-Dashboard für diese Benutzer</span><span class="sxs-lookup"><span data-stu-id="106cb-116">Remove access to the sitemap defined dashboard for those users</span></span>
