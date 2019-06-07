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
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer Verbindungsprobleme 

Wenn bei SharePoint Designer Verbindungsprobleme mit SharePoint-Websites auftreten, versuchen Sie die folgenden gängigen Lösungen.

Schritt 1: überprüfen, ob SharePoint Designer aktualisiert wurde.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Update für SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Schritt 2: Löschen der lokalen Cachedateien

- Schließen Sie SharePoint Designer 2013.

- Wechseln Sie auf dem lokalen Computer zu den folgenden Ordnern, um zwischengespeicherte Dateien zu entfernen.

- Klicken Sie auf Start, führen Sie aus, und löschen Sie alle Dateien, die unter jeder der unten aufgeführten Speicherorte gefunden wurden.

%APPDATA%\Microsoft\Web Server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Öffnen Sie SharePoint Designer 2013, und geben Sie das Konto erneut ein, um zu sehen, ob es funktioniert.

Schritt 3: [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Schritt 4: Administratoren müssen zulassen, dass das benutzerdefinierte Skript die SharePoint Designer Verbindung zulässt.

Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


