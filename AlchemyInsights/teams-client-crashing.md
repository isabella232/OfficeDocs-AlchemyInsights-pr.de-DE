---
title: Teams-Client stürzt ab?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030584"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="1316c-102">Teams-Client stürzt ab?</span><span class="sxs-lookup"><span data-stu-id="1316c-102">Teams client crashing?</span></span>

<span data-ttu-id="1316c-103">Wenn Ihr Team-Client abstürzt, versuchen Sie bitte Folgendes:</span><span class="sxs-lookup"><span data-stu-id="1316c-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="1316c-104">Wenn Sie die Team-Desktop-App verwenden, [Stellen Sie sicher, dass die App vollständig aktualisiert wurde](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="1316c-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="1316c-105">Stellen Sie sicher, dass auf alle [Office 365-URLs und-Adressbereiche](https://docs.microsoft.com/microsoftteams/connectivity-issues) zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="1316c-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="1316c-106">Melden Sie sich mit Ihrem Administratorkonto an und überprüfen Sie in Ihrem [Dienststatus-Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health), ob ein Ausfall oder eine Verschlechterung des Dienstes eingetreten ist.</span><span class="sxs-lookup"><span data-stu-id="1316c-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="1316c-107">Als letzten Schritt können Sie versuchen, den Clientcache für Teams zu löschen:</span><span class="sxs-lookup"><span data-stu-id="1316c-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="1316c-108">Steigen Sie vollständig aus dem Desktop-Client für Microsoft Teams aus.</span><span class="sxs-lookup"><span data-stu-id="1316c-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="1316c-109">Sie können mit der rechten Maustaste in der Taskleiste auf **Teams** klicken und dann **Beenden** anklicken oder den Task-Manager ausführen und den Vorgang vollständig beenden.</span><span class="sxs-lookup"><span data-stu-id="1316c-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="1316c-110">Wechseln Sie zum Datei-Explorer, und geben Sie „%appdata%\Microsoft\teams“ ein.</span><span class="sxs-lookup"><span data-stu-id="1316c-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="1316c-111">Sobald Sie sich im Verzeichnis befinden, werden einige der folgenden Ordner angezeigt:</span><span class="sxs-lookup"><span data-stu-id="1316c-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="1316c-112">Wechseln Sie im**Anwendungscache** zum Cache und löschen Sie alle darin befindlichen Dateien: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="1316c-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="1316c-113">Löschen Sie alle Dateien im **Blob_Speicher**: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="1316c-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="1316c-114">Löschen Sie alle Dateien im **Cache**: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="1316c-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="1316c-115">Löschen Sie alle Dateien in den **Datenbanken**: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="1316c-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="1316c-116">Löschen Sie alle Dateien im **GPU-Cache**: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="1316c-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="1316c-117">Löschen Sie die .db-Datei in der **Indexierten DB**: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="1316c-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="1316c-118">Löschen Sie alle Dateien im **Lokalen Speicher**: %appdata%\Microsoft\teams\Local_Storage.</span><span class="sxs-lookup"><span data-stu-id="1316c-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="1316c-119">Und als letzten Schritt löschen Sie alle Dateien aus dem **TEMP-Verzeichnis**: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="1316c-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="1316c-120">Starten Sie den Teams-Client neu.</span><span class="sxs-lookup"><span data-stu-id="1316c-120">Restart your Teams client.</span></span>
