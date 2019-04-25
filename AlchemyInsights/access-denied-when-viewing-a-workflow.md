---
title: Zugriff verweigert beim Anzeigen eines Workflows
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389886"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff verweigert beim Anzeigen eines Workflows

SharePoint 2013-Workflows, die versuchen, eine e-Mail an eine SharePoint-Gruppe zu senden, können mit einer Fehlermeldung "Zugriff verweigert" fehlschlagen, wenn die Mitgliedschaft in der SharePoint-Gruppe nicht auf jeder festgelegt ist.
  
 **Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**
  
 1. Zulassen, dass alle Mitglieder der SharePoint-Gruppe angezeigt werden. 
  
 2. Entfernen Sie die SharePoint-Gruppe aus der an-oder CC-Zeile der e-Mail. 
  
 3. Fügen Sie die Benutzer explizit der Zeile an oder CC hinzu, wenn die Mitgliedschafts Sichtbarkeit für die SharePoint-Gruppe nicht geändert werden kann. 
  
Weitere Informationen finden Sie unter unAuthorized [to/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

