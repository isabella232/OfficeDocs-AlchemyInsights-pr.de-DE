---
title: Moderne Website als Stammwebsite
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057711"
---
# <a name="modern-site-as-root-site"></a>Moderne Website als Stammwebsite

[Ziel Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) -Kunden können jetzt die moderne Kommunikationswebsite auf der klassischen Stammwebsite Ihres SharePoint-Mandanten aktivieren.

Dieses Feature kann durch Ausführen eines einfachen PowerShell-Cmdlets aktiviert werden. Bei erfolgreicher Ausführung der PowerShell-Befehle verfügt die Stammwebsite über eine neue Homepage für die Kommunikationswebsite. Details zu den PowerShell-Cmdlets und Funktionsanforderungen finden Sie im Artikel [enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Nach und nach werden wir das in der Standardeinstellung für Zielversionen von Kunden Anfang Mai 2019 und die Einführung weltweit bis Ende Juni 2019 zur Verfügung stellen. Weitere Informationen finden Sie im [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) für andere neue Features mit modern. 

**Wichtig**: Löschen Sie Ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen. Dies wird von Microsoft nicht unterstützt. Durch das Löschen der Stammwebsite werden alle SharePoint-Websites in Ihrer Organisation für alle Benutzer unzugänglich, bis Sie die Website wiederherstellen oder eine neue Website mit derselben URL erstellen. 
 
 