---
title: Teams-Client stürzt ab?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826270"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="20e45-102">Teams-Client stürzt ab?</span><span class="sxs-lookup"><span data-stu-id="20e45-102">Teams client crashing?</span></span>

<span data-ttu-id="20e45-103">Wenn Ihr Team-Client abstürzt, versuchen Sie bitte Folgendes:</span><span class="sxs-lookup"><span data-stu-id="20e45-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="20e45-104">Wenn Sie die Team-Desktop-App verwenden, [Stellen Sie sicher, dass die App vollständig aktualisiert wurde](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="20e45-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="20e45-105">Stellen Sie sicher, dass auf alle [Microsoft 365-URLs und -Adressbereiche](https://docs.microsoft.com/microsoftteams/connectivity-issues) zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="20e45-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="20e45-106">Melden Sie sich mit Ihrem Mandanten-Administratorkonto an und überprüfen Sie in Ihrem [Dienststatus-Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health), ob ein Ausfall oder eine Verschlechterung des Dienstes eingetreten ist.</span><span class="sxs-lookup"><span data-stu-id="20e45-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="20e45-107">Deinstallieren und erneutes Installieren der Microsoft Teams-Anwendung (Link)</span><span class="sxs-lookup"><span data-stu-id="20e45-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="20e45-108">Navigieren Sie zum Ordner „%appdata%\Microsoft\teams\“ auf Ihrem Computer, und löschen Sie alle Dateien in diesem Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="20e45-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="20e45-109">[Laden Sie die Microsoft Teams-App herunter, und installieren Sie sie](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy). Installieren Sie Microsoft Teams dabei nach Möglichkeit als Administrator (Klicken Sie mit der rechten Maustaste auf das Installationsprogramm für Microsoft Teams, und wählen Sie, sofern verfügbar, "Als Administrator ausführen" aus).</span><span class="sxs-lookup"><span data-stu-id="20e45-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="20e45-110">Wenn Ihr Microsoft Teams-Client weiterhin abstürzt, können Sie das Problem reproduzieren?</span><span class="sxs-lookup"><span data-stu-id="20e45-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="20e45-111">Wenn ja, tun Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="20e45-111">If so:</span></span>

1. <span data-ttu-id="20e45-112">Erfassen Sie mithilfe des Steps Recorders Ihre Schritte.</span><span class="sxs-lookup"><span data-stu-id="20e45-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="20e45-113">Schließen Sie ALLE unnötigen oder vertraulichen Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="20e45-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="20e45-114">Starten Sie den Steps Recorder, und reproduzieren Sie das Problem, während Sie in dem betroffenen Benutzerkonto angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="20e45-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="20e45-115">[Sammeln Sie die Microsoft Teams-Protokolle, die die aufgezeichneten Reproduktionsschritte enthalten](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="20e45-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="20e45-116">**Hinweis**: Vergewissern Sie sich, dass Sie die Anmeldeadresse des betroffenen Benutzers erfassen.</span><span class="sxs-lookup"><span data-stu-id="20e45-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="20e45-117">Sammeln Sie die Abbild- und/oder Fehler-Bucket-Informationen (Windows).</span><span class="sxs-lookup"><span data-stu-id="20e45-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="20e45-118">Starten Sie Windows PowerShell auf dem Computer, auf dem der Absturz erfolgt, und führen Sie die folgenden Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="20e45-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="20e45-119">Fügen Sie die Datei an Ihren Supportfall an.</span><span class="sxs-lookup"><span data-stu-id="20e45-119">Attach the file to your support case.</span></span>
