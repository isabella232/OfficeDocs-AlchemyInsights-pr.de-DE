---
title: Profilsynchronisierung
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768112"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wann wird meine Profiländerung mit der SharePoint-benutzerprofilanwendung synchronisiert?

SharePoint Online verwendet den Active Directory Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in die benutzerprofilanwendung zu importieren. 
  
1. Durch AD-Import werden Änderungen aus dem SharePoint Online Verzeichnisspeicher in die benutzerprofilanwendung synchronisiert. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.
    
> [!NOTE]
> Die Zeit, die für die Ausführung des Auftrags erforderlich ist, hängt von der Anzahl der zu verarbeitenden Änderungen ab. Eine große Anzahl von Änderungen dauert länger. Die Vereinbarung zum Service Level (SLA) besagt, dass sich eine Änderung an einem Benutzer im SharePoint Online-Verzeichnis in der benutzerprofilanwendung in 24 Stunden widerspiegelt. 
  
[Weitere Informationen zur Benutzerprofil Synchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

