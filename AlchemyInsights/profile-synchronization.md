---
title: Profilsynchronisierung
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371983"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wann ändert mein Profil die Synchronisierung mit der SharePoint-Benutzerprofilanwendung?

SharePoint Online verwendet den Active Directory-Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in die Benutzerprofilanwendung zu importieren. 
  
1. Der AD-Import synchronisiert Änderungen vom SharePoint Online-Verzeichnisspeicher zur Benutzerprofilanwendung. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.
    
> [!NOTE]
> Die Zeit, die der Auftrag ausgeführt wird, hängt von der Anzahl der zu verarbeitenden Änderungen ab. Eine größere Anzahl von Änderungen dauert länger. Die Vereinbarung zum Service Level (SLA) besagt, dass eine Änderung an einem Benutzer im SharePoint Online-Verzeichnis in 24 Stunden in der Benutzerprofilanwendung wiedergegeben wird. 
  
[Weitere Informationen zur Benutzerprofil Synchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

