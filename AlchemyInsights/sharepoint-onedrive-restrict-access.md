---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692764"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0d598-102">Einschränken des Zugriffs in SharePoint oder OneDrive</span><span class="sxs-lookup"><span data-stu-id="0d598-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0d598-103">Es gibt viele Möglichkeiten, den Zugriff auf SharePoint Online/OneDrive-Dienste einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="0d598-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="0d598-104">Diese verschiedenen Methoden zur Zugriffseinschränkung werden weiter unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="0d598-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="0d598-105">**Berechtigungs Beschränkung**</span><span class="sxs-lookup"><span data-stu-id="0d598-105">**Permission Restriction**</span></span>

<span data-ttu-id="0d598-106">In SharePoint Online und OneDrive für Unternehmen beschränken wir den Zugriff auf Elemente wie Websites, Dateien und Ordner, indem wir nur Zugriff auf diese Gruppen/Personen gewähren, die Zugriff haben sollten.</span><span class="sxs-lookup"><span data-stu-id="0d598-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="0d598-107">Anpassen von Berechtigungen für eine SharePoint-Liste oder-Bibliothek</span><span class="sxs-lookup"><span data-stu-id="0d598-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="0d598-108">Anpassen von SharePoint-Websiteberechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d598-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="0d598-109">Ändern der Berechtigungen für einen Unterordner</span><span class="sxs-lookup"><span data-stu-id="0d598-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="0d598-110">Steuern des Zugriffs von nicht verwalteten Geräten</span><span class="sxs-lookup"><span data-stu-id="0d598-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="0d598-111">Als SharePoint-oder globaler Administrator können Sie den Zugriff auf SharePoint-und OneDrive-Inhalte von nicht verwalteten Geräten (die nicht mit Hybrid-AD verbunden oder in InTune kompatibel sind) blockieren oder einschränken.</span><span class="sxs-lookup"><span data-stu-id="0d598-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="0d598-112">**Einschränkung des Netzwerkstandorts**</span><span class="sxs-lookup"><span data-stu-id="0d598-112">**Network Location Restriction**</span></span>

<span data-ttu-id="0d598-113">Als IT-Administrator können Sie den Zugriff auf SharePoint-und OneDrive-Ressourcen basierend auf definierten Netzwerkstandorten steuern, denen Sie vertrauen.</span><span class="sxs-lookup"><span data-stu-id="0d598-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="0d598-114">Dies wird auch als standortbasierte Richtlinie bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="0d598-114">This is also known as location-based policy.</span></span> <span data-ttu-id="0d598-115">Weitere Informationen finden Sie unter [Steuern des Zugriffs auf SharePoint Online-und OneDrive-Daten basierend auf dem Netzwerkstandort](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .</span><span class="sxs-lookup"><span data-stu-id="0d598-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="0d598-116">**Einschränkung der Website Sperre**</span><span class="sxs-lookup"><span data-stu-id="0d598-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="0d598-117">In SharePoint Online haben Sie die Möglichkeit, eine Websitesammlung zu sperren, sodass niemand Zugriff hat.</span><span class="sxs-lookup"><span data-stu-id="0d598-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="0d598-118">Dies wird über PowerShell und die [SharePoint Online-Verwaltungsshell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) mithilfe der Eigenschaft " [Sets-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0d598-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="0d598-119">**Einschränken der Benutzer am Erstellen von Websites oder Unterwebsites**</span><span class="sxs-lookup"><span data-stu-id="0d598-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="0d598-120">Als SharePoint-Administrator oder globaler Administrator können Sie Ihren Benutzern die Erstellung und Verwaltung Ihrer eigenen SharePoint-Websites ermöglichen, bestimmen, welche Art von Websites Sie erstellen können, und den Speicherort der Websites angeben.</span><span class="sxs-lookup"><span data-stu-id="0d598-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="0d598-121">Weitere Informationen finden Sie unter [Manage Site Creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="0d598-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

