---
title: Entfernen des Hintergrunddienstes für Microsoft Search in Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753415"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="4e2d8-102">Entfernen des Hintergrunddienstes für Microsoft Search in Bing</span><span class="sxs-lookup"><span data-stu-id="4e2d8-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="4e2d8-103">Um den Hintergrunddienst für Microsoft Search in Bing zu entfernen, können Sie folgende Möglichkeiten versuchen:</span><span class="sxs-lookup"><span data-stu-id="4e2d8-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="4e2d8-104">Um zu den ursprünglichen Suchmaschinen-Einstellungen zurückzukehren, führen Sie Folgendes durch:</span><span class="sxs-lookup"><span data-stu-id="4e2d8-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="4e2d8-105">a.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-105">a.</span></span> <span data-ttu-id="4e2d8-106">Setzen Sie den Schalter **Bing als Standardsuchmaschine verwenden [auf](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Aus**.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="4e2d8-107">b.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-107">b.</span></span> <span data-ttu-id="4e2d8-108">[Gehen Sie zum Microsoft 365 Admin Center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) und löschen Sie die Einstellung, welche alle Benutzer in Ihrer Organisation betrifft.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="4e2d8-109">Um den Hintergrunddienst von einem einzelnen Gerät zu entfernen, führen Sie folgende Tasks durch:</span><span class="sxs-lookup"><span data-stu-id="4e2d8-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="4e2d8-110">a.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-110">a.</span></span> <span data-ttu-id="4e2d8-111">Wählen Sie **Systemsteuerung > Programme > Programme und Funktionen** aus.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="4e2d8-112">b.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-112">b.</span></span> <span data-ttu-id="4e2d8-113">Klicken Sie in der Liste der installierten Programme mit der rechten Maustaste auf **Microsoft Search in Bing**, und anschließend klicken Sie auf **Deinstallieren**.</span><span class="sxs-lookup"><span data-stu-id="4e2d8-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="4e2d8-114">Um den Hintergrunddienst von mehreren Geräten in Ihrer Organisation zu entfernen, melden Sie sich als Administrator an und führen Sie den folgenden Befehl in einem Skript aus:</span><span class="sxs-lookup"><span data-stu-id="4e2d8-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
