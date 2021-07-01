---
title: Teams-Client stürzt ab
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187720"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="c2eeb-102">Teams-Client stürzt ab</span><span class="sxs-lookup"><span data-stu-id="c2eeb-102">Teams client crashing</span></span>

<span data-ttu-id="c2eeb-103">Wenn Ihr Team-Client abstürzt, versuchen Sie bitte Folgendes:</span><span class="sxs-lookup"><span data-stu-id="c2eeb-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="c2eeb-104">Wenn Sie die Team-Desktop-App verwenden, [Stellen Sie sicher, dass die App vollständig aktualisiert wurde](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="c2eeb-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="c2eeb-105">Stellen Sie sicher, dass auf alle [Microsoft 365-URLs und -Adressbereiche](/microsoftteams/connectivity-issues) zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="c2eeb-106">Melden Sie sich mit Ihrem Mandanten-Administratorkonto an und überprüfen Sie in Ihrem [Dienststatus-Dashboard](/office365/enterprise/view-service-health), ob ein Ausfall oder eine Verschlechterung des Dienstes eingetreten ist.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="c2eeb-107">Deinstallieren und erneutes Installieren der Microsoft Teams-Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2eeb-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="c2eeb-108">Navigieren Sie zum Ordner „%appdata%\Microsoft\Teams\“ auf Ihrem Computer, und löschen Sie alle Dateien in diesem Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="c2eeb-109">[Laden Sie die Microsoft Teams-App herunter, und installieren Sie sie](https://www.microsoft.com/microsoft-teams/download-app). Installieren Sie Microsoft Teams dabei nach Möglichkeit als Administrator (Klicken Sie mit der rechten Maustaste auf das Installationsprogramm für Microsoft Teams, und wählen Sie, sofern verfügbar, **Als Administrator ausführen** aus).</span><span class="sxs-lookup"><span data-stu-id="c2eeb-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="c2eeb-110">Wenn Ihr Microsoft Teams-Client weiterhin abstürzt, versuchen Sie, das Problem zu reproduzieren.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="c2eeb-111">Ist dies möglich:</span><span class="sxs-lookup"><span data-stu-id="c2eeb-111">If you can:</span></span>

1. <span data-ttu-id="c2eeb-112">Erfassen Sie mithilfe des Steps Recorders Ihre Schritte.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="c2eeb-113">Schließen Sie ALLE unnötigen oder vertraulichen Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="c2eeb-114">Starten Sie den Steps Recorder, und reproduzieren Sie das Problem, während Sie in dem betroffenen Benutzerkonto angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="c2eeb-115">[Sammeln Sie die Microsoft Teams-Protokolle, die die aufgezeichneten Reproduktionsschritte enthalten](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="c2eeb-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="c2eeb-116">**Hinweis**: Vergewissern Sie sich, dass Sie die Anmeldeadresse des betroffenen Benutzers erfassen.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="c2eeb-117">Sammeln Sie die Abbild- und/oder Fehler-Bucket-Informationen (Windows).</span><span class="sxs-lookup"><span data-stu-id="c2eeb-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="c2eeb-118">Starten Sie Windows PowerShell auf dem Computer, auf dem der Absturz erfolgt, und führen Sie die folgenden Befehle aus (drücken Sie nach jedem Befehl die EINGABETASTE):</span><span class="sxs-lookup"><span data-stu-id="c2eeb-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="c2eeb-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="c2eeb-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="c2eeb-120">Nachdem die Textdatei generiert wurde und auf dem Bildschirm angezeigt wird, speichern Sie die Datei, und fügen Sie sie an die Serviceanfrage an.</span><span class="sxs-lookup"><span data-stu-id="c2eeb-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
