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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470392"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5038d-102">Wenn führen Sie Mein Profil Änderungen an der SharePoint-Benutzerprofilanwendung synchronisieren?</span><span class="sxs-lookup"><span data-stu-id="5038d-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5038d-103">SharePoint Online verwendet den Active Directory-Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in der Benutzerprofildienst-Anwendung zu importieren.</span><span class="sxs-lookup"><span data-stu-id="5038d-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5038d-p101">AD-Import synchronisiert Änderungen aus dem Verzeichnisspeicher für SharePoint Online auf die Benutzerprofildienst-Anwendung. Diese Änderungen werden in Batches verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="5038d-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5038d-106">Der Zeitgeberauftrag ausgeführt wird, bis die Änderungen synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="5038d-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5038d-p102">Die Ausführung des Auftrags erforderliche Zeit hängt von der Anzahl von Änderungen an verarbeiten. Eine große Anzahl von Änderungen dauert länger. Service Level Agreement (SLA) gibt an, dass eine Änderung für einen Benutzer in SharePoint Online-Verzeichnis in die Benutzerprofildienst-Anwendung in 24 Stunden widergespiegelt werden.</span><span class="sxs-lookup"><span data-stu-id="5038d-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5038d-110">Weitere Informationen zum Benutzer profilsynchronisierung in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5038d-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

