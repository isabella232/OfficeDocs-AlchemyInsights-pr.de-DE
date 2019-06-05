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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716891"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer Verbindungsprobleme 

<p>Wenn bei SharePoint Designer Verbindungsprobleme mit SharePoint-Websites auftreten, versuchen Sie die folgenden gängigen Lösungen.</p> <p><strong>Schritt 1:</strong> <strong>Überprüfen, ob&nbsp; SharePoint Designer aktualisiert wurde</strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Update für SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Schritt 2:</strong> <strong>Löschen der lokalen Cachedateien</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Schließen Sie SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Wechseln Sie auf dem lokalen Computer zu den folgenden Ordnern, um zwischengespeicherte Dateien zu entfernen.&nbsp;</li> <li style="font-weight: 400;">Klicken Sie auf <strong>Start-&gt; Run</strong> , und löschen Sie alle Dateien, die unter den folgenden Speicherorten gefunden wurden.&nbsp;<br /><br />%APPDATA%\Microsoft\Web-Server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Öffnen Sie SharePoint Designer 2013, und geben Sie das Konto erneut ein, um zu sehen, ob es funktioniert.</li> </ol> <p><strong>Schritt 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten</strong></a>&nbsp;</p> <p><strong>Schritt 4:</strong> <strong>Administratoren müssen zulassen, dass das benutzerdefinierte Skript die SharePoint Designer Verbindung zulässt</strong>.</p> <p>Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">zulassen oder verhindern von benutzerdefiniertem Skript</a>.&nbsp;</p>


