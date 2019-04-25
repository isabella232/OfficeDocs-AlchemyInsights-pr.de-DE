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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5b6a8-102">Wann ändert mein Profil die Synchronisierung mit der SharePoint-Benutzerprofilanwendung?</span><span class="sxs-lookup"><span data-stu-id="5b6a8-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5b6a8-103">SharePoint Online verwendet den Active Directory-Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in die Benutzerprofilanwendung zu importieren.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5b6a8-104">Der AD-Import synchronisiert Änderungen vom SharePoint Online-Verzeichnisspeicher zur Benutzerprofilanwendung.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="5b6a8-105">Diese Änderungen werden in Batches verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5b6a8-106">Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5b6a8-107">Die Zeit, die der Auftrag ausgeführt wird, hängt von der Anzahl der zu verarbeitenden Änderungen ab.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="5b6a8-108">Eine größere Anzahl von Änderungen dauert länger.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-108">A large number of changes takes longer.</span></span> <span data-ttu-id="5b6a8-109">Die Vereinbarung zum Service Level (SLA) besagt, dass eine Änderung an einem Benutzer im SharePoint Online-Verzeichnis in 24 Stunden in der Benutzerprofilanwendung wiedergegeben wird.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5b6a8-110">Weitere Informationen zur Benutzerprofil Synchronisierung in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5b6a8-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

