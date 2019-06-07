---
title: SharePoint Online Berechtigungsstufen
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760692"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="431a9-102">SharePoint Designer Verbindungsprobleme</span><span class="sxs-lookup"><span data-stu-id="431a9-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="431a9-103">Wenn bei SharePoint Designer Verbindungsprobleme mit SharePoint-Websites auftreten, versuchen Sie die folgenden gängigen Lösungen.</span><span class="sxs-lookup"><span data-stu-id="431a9-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="431a9-104">Schritt 1: überprüfen, ob SharePoint Designer aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="431a9-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="431a9-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="431a9-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="431a9-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="431a9-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="431a9-107">Update für SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="431a9-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="431a9-108">Schritt 2: Löschen der lokalen Cachedateien</span><span class="sxs-lookup"><span data-stu-id="431a9-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="431a9-109">Schließen Sie SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="431a9-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="431a9-110">Wechseln Sie auf dem lokalen Computer zu den folgenden Ordnern, um zwischengespeicherte Dateien zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="431a9-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="431a9-111">Klicken Sie auf Start, führen Sie aus, und löschen Sie alle Dateien, die unter jeder der unten aufgeführten Speicherorte gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="431a9-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="431a9-112">%APPDATA%\Microsoft\Web Server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="431a9-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="431a9-113">Öffnen Sie SharePoint Designer 2013, und geben Sie das Konto erneut ein, um zu sehen, ob es funktioniert.</span><span class="sxs-lookup"><span data-stu-id="431a9-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="431a9-114">Schritt 3: [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="431a9-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="431a9-115">Schritt 4: Administratoren müssen zulassen, dass das benutzerdefinierte Skript die SharePoint Designer Verbindung zulässt.</span><span class="sxs-lookup"><span data-stu-id="431a9-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="431a9-116">Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="431a9-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


