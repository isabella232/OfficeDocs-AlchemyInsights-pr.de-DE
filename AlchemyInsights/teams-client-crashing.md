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
# <a name="teams-client-crashing"></a>Teams-Client stürzt ab?

Wenn Ihr Team-Client abstürzt, versuchen Sie bitte Folgendes:

- Wenn Sie die Team-Desktop-App verwenden, [Stellen Sie sicher, dass die App vollständig aktualisiert wurde](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Stellen Sie sicher, dass auf alle [Microsoft 365-URLs und -Adressbereiche](https://docs.microsoft.com/microsoftteams/connectivity-issues) zugegriffen werden kann.

- Melden Sie sich mit Ihrem Mandanten-Administratorkonto an und überprüfen Sie in Ihrem [Dienststatus-Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health), ob ein Ausfall oder eine Verschlechterung des Dienstes eingetreten ist.

- Deinstallieren und erneutes Installieren der Microsoft Teams-Anwendung (Link)
    - Navigieren Sie zum Ordner „%appdata%\Microsoft\teams\“ auf Ihrem Computer, und löschen Sie alle Dateien in diesem Verzeichnis.
    - [Laden Sie die Microsoft Teams-App herunter, und installieren Sie sie](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy). Installieren Sie Microsoft Teams dabei nach Möglichkeit als Administrator (Klicken Sie mit der rechten Maustaste auf das Installationsprogramm für Microsoft Teams, und wählen Sie, sofern verfügbar, "Als Administrator ausführen" aus).

Wenn Ihr Microsoft Teams-Client weiterhin abstürzt, können Sie das Problem reproduzieren? Wenn ja, tun Sie Folgendes:

1. Erfassen Sie mithilfe des Steps Recorders Ihre Schritte.
    - Schließen Sie ALLE unnötigen oder vertraulichen Anwendungen.
    - Starten Sie den Steps Recorder, und reproduzieren Sie das Problem, während Sie in dem betroffenen Benutzerkonto angemeldet sind.
    - [Sammeln Sie die Microsoft Teams-Protokolle, die die aufgezeichneten Reproduktionsschritte enthalten](https://docs.microsoft.com/microsoftteams/log-files). **Hinweis**: Vergewissern Sie sich, dass Sie die Anmeldeadresse des betroffenen Benutzers erfassen.
    - Sammeln Sie die Abbild- und/oder Fehler-Bucket-Informationen (Windows). Starten Sie Windows PowerShell auf dem Computer, auf dem der Absturz erfolgt, und führen Sie die folgenden Befehle aus:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Fügen Sie die Datei an Ihren Supportfall an.
