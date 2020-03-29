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
# <a name="teams-client-crashing"></a>Teams-Client stürzt ab?

Wenn Ihr Team-Client abstürzt, versuchen Sie bitte Folgendes:

- Wenn Sie die Team-Desktop-App verwenden, [Stellen Sie sicher, dass die App vollständig aktualisiert wurde](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Stellen Sie sicher, dass auf alle [Office 365-URLs und-Adressbereiche](https://docs.microsoft.com/microsoftteams/connectivity-issues) zugegriffen werden kann.

- Melden Sie sich mit Ihrem Administratorkonto an und überprüfen Sie in Ihrem [Dienststatus-Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health), ob ein Ausfall oder eine Verschlechterung des Dienstes eingetreten ist.

 - Als letzten Schritt können Sie versuchen, den Clientcache für Teams zu löschen:

    1.  Steigen Sie vollständig aus dem Desktop-Client für Microsoft Teams aus. Sie können mit der rechten Maustaste in der Taskleiste auf **Teams** klicken und dann **Beenden** anklicken oder den Task-Manager ausführen und den Vorgang vollständig beenden.

    2.  Wechseln Sie zum Datei-Explorer, und geben Sie „%appdata%\Microsoft\teams“ ein.

    3.  Sobald Sie sich im Verzeichnis befinden, werden einige der folgenden Ordner angezeigt:

         - Wechseln Sie im**Anwendungscache** zum Cache und löschen Sie alle darin befindlichen Dateien: %appdata%\Microsoft\teams\application cache\cache.

        - Löschen Sie alle Dateien im **Blob_Speicher**: %appdata%\Microsoft\teams\blob_storage.

        - Löschen Sie alle Dateien im **Cache**: %appdata%\Microsoft\teams\Cache.

        - Löschen Sie alle Dateien in den **Datenbanken**: %appdata%\Microsoft\teams\databases.

        - Löschen Sie alle Dateien im **GPU-Cache**: %appdata%\Microsoft\teams\GPUcache.

        - Löschen Sie die .db-Datei in der **Indexierten DB**: %appdata%\Microsoft\teams\IndexedDB.

        - Löschen Sie alle Dateien im **Lokalen Speicher**: %appdata%\Microsoft\teams\Local_Storage.

        - Und als letzten Schritt löschen Sie alle Dateien aus dem **TEMP-Verzeichnis**: %appdata%\Microsoft\teams\tmp.

    4. Starten Sie den Teams-Client neu.
