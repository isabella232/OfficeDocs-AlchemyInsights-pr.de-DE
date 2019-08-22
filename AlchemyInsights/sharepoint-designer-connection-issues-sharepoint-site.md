---
title: SharePoint Designer Verbindungsprobleme
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508422"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="b5643-102">SharePoint Designer Verbindungsprobleme</span><span class="sxs-lookup"><span data-stu-id="b5643-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="b5643-103">Wenn bei SharePoint Designer Verbindungsprobleme mit SharePoint-Websites auftreten, versuchen Sie es mit den folgenden gängigen Lösungen.</span><span class="sxs-lookup"><span data-stu-id="b5643-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="b5643-104">Schritt 1: Stellen Sie sicher, dass SharePoint Designer 2013 mit [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) und dem [Update vom August 2 2016 aktualisiert wurde, um SharePoint Designer 2013 zu aktualisieren](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="b5643-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="b5643-105">Schritt 2: Löschen der lokalen Cachedateien:</span><span class="sxs-lookup"><span data-stu-id="b5643-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="b5643-106">Schließen Sie SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b5643-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="b5643-107">Entfernen Sie auf dem lokalen Computer alle Dateien, die in den folgenden Ordnern gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="b5643-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="b5643-108">%APPDATA%\Microsoft\Web-Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="b5643-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="b5643-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="b5643-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="b5643-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="b5643-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="b5643-111">Öffnen Sie SharePoint Designer 2013, und geben Sie das Konto erneut ein, um zu sehen, ob es funktioniert.</span><span class="sxs-lookup"><span data-stu-id="b5643-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="b5643-112">Schritt 3: [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b5643-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="b5643-113">Schritt 4: Administratoren müssen **benutzerdefiniertes Skript** in den SharePoint Admin Center-Einstellungen zulassen, um die SharePoint Designer Verbindung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="b5643-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="b5643-114">Weitere Informationen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="b5643-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


