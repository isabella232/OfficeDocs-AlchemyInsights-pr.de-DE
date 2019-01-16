---
title: Profilsynchronisierung
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289568"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wenn führen Sie Mein Profil Änderungen an der SharePoint-Benutzerprofilanwendung synchronisieren?

SharePoint Online verwendet den Active Directory-Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in der Benutzerprofildienst-Anwendung zu importieren. 
  
1. AD-Import synchronisiert Änderungen aus dem Verzeichnisspeicher für SharePoint Online auf die Benutzerprofildienst-Anwendung. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag ausgeführt wird, bis die Änderungen synchronisiert werden.
    
> [!NOTE]
> Die Ausführung des Auftrags erforderliche Zeit hängt von der Anzahl von Änderungen an verarbeiten. Eine große Anzahl von Änderungen dauert länger. Service Level Agreement (SLA) gibt an, dass eine Änderung für einen Benutzer in SharePoint Online-Verzeichnis in die Benutzerprofildienst-Anwendung in 24 Stunden widergespiegelt werden. 
  
[Weitere Informationen zum Benutzer profilsynchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

