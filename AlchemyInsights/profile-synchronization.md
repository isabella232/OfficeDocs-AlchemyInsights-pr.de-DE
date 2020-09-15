---
title: Profilsynchronisierung
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801768"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wann wird meine Profiländerung mit der SharePoint-benutzerprofilanwendung synchronisiert?

SharePoint Online verwendet den Active Directory Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in die benutzerprofilanwendung zu importieren. 
  
1. Durch AD-Import werden Änderungen aus dem SharePoint Online Verzeichnisspeicher in die benutzerprofilanwendung synchronisiert. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.
    
> [!NOTE]
> Die Zeit, die für die Ausführung des Auftrags erforderlich ist, hängt von der Anzahl der zu verarbeitenden Änderungen ab. Eine große Anzahl von Änderungen dauert länger. Die Vereinbarung zum Service Level (SLA) besagt, dass sich eine Änderung an einem Benutzer im SharePoint Online-Verzeichnis in der benutzerprofilanwendung in 24 Stunden widerspiegelt. 
  
[Weitere Informationen zur Benutzerprofil Synchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

