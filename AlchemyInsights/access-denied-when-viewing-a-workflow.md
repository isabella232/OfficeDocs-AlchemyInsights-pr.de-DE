---
title: Zugriff verweigert beim Anzeigen eines Workflows
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289258"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="9e4fd-102">Zugriff verweigert beim Anzeigen eines Workflows</span><span class="sxs-lookup"><span data-stu-id="9e4fd-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="9e4fd-103">SharePoint 2013-Workflows, die versuchen, eine e-Mail an eine SharePoint-Gruppe senden können mit einer Fehlermeldung "Zugriff verweigert" fehl, wenn die Mitgliedschaft der SharePoint-Gruppe nicht auf jeder festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="9e4fd-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="9e4fd-104">**Um dieses Problem zu beheben, führen Sie diese Schritte aus:**</span><span class="sxs-lookup"><span data-stu-id="9e4fd-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="9e4fd-105">Erlauben Sie allen Mitgliedern der Mitglieder der SharePoint-Gruppe finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="9e4fd-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="9e4fd-106">Entfernen die SharePoint-Gruppe aus "an" oder "Cc" Zeile der e-Mail.</span><span class="sxs-lookup"><span data-stu-id="9e4fd-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="9e4fd-107">Die Benutzer explizit an oder CC hinzufügen auszurichten, wenn die Sichtbarkeit der Mitgliedschaft für SharePoint-Gruppe nicht geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="9e4fd-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="9e4fd-108">Zum Anzeigen von finden Sie weitere Details auf [HTTP unbefugte zu /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9e4fd-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

