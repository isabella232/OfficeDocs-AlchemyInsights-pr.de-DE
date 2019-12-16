---
title: Zugriff verweigert beim Anzeigen eines Workflows
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050524"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="8615a-102">Zugriff verweigert beim Anzeigen eines Workflows</span><span class="sxs-lookup"><span data-stu-id="8615a-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="8615a-103">SharePoint 2013 Workflows, die versuchen, eine e-Mail an eine SharePoint-Gruppe zu senden, können mit der Fehlermeldung "Zugriff verweigert" fehlschlagen, wenn die Mitgliedschaft in der SharePoint-Gruppe nicht auf jeder festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="8615a-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="8615a-104">**Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**</span><span class="sxs-lookup"><span data-stu-id="8615a-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="8615a-105">Lassen Sie alle Mitglieder der SharePoint-Gruppe anzeigen.</span><span class="sxs-lookup"><span data-stu-id="8615a-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="8615a-106">Entfernen Sie die SharePoint-Gruppe aus der an-oder CC-Zeile der e-Mail.</span><span class="sxs-lookup"><span data-stu-id="8615a-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="8615a-107">Fügen Sie die Benutzer explizit zur Zeile "an" oder "CC" hinzu, wenn die Mitgliedschafts Sichtbarkeit für SharePoint-Gruppe nicht geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="8615a-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="8615a-108">Weitere Informationen finden Sie unter [http Authorized to/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8615a-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  