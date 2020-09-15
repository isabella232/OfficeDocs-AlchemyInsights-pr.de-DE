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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="e0172-102">Wann wird meine Profiländerung mit der SharePoint-benutzerprofilanwendung synchronisiert?</span><span class="sxs-lookup"><span data-stu-id="e0172-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="e0172-103">SharePoint Online verwendet den Active Directory Import-Zeitgeberauftrag (AD-Import), um Benutzer und Gruppen in die benutzerprofilanwendung zu importieren.</span><span class="sxs-lookup"><span data-stu-id="e0172-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="e0172-104">Durch AD-Import werden Änderungen aus dem SharePoint Online Verzeichnisspeicher in die benutzerprofilanwendung synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="e0172-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="e0172-105">Diese Änderungen werden in Batches verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="e0172-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="e0172-106">Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="e0172-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="e0172-107">Die Zeit, die für die Ausführung des Auftrags erforderlich ist, hängt von der Anzahl der zu verarbeitenden Änderungen ab.</span><span class="sxs-lookup"><span data-stu-id="e0172-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="e0172-108">Eine große Anzahl von Änderungen dauert länger.</span><span class="sxs-lookup"><span data-stu-id="e0172-108">A large number of changes takes longer.</span></span> <span data-ttu-id="e0172-109">Die Vereinbarung zum Service Level (SLA) besagt, dass sich eine Änderung an einem Benutzer im SharePoint Online-Verzeichnis in der benutzerprofilanwendung in 24 Stunden widerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="e0172-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="e0172-110">Weitere Informationen zur Benutzerprofil Synchronisierung in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e0172-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

