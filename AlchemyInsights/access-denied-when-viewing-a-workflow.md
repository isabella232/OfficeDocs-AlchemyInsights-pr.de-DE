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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918827"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff verweigert beim Anzeigen eines Workflows

SharePoint 2013-Workflows, die versuchen, eine e-Mail an eine SharePoint-Gruppe senden können mit einer Fehlermeldung "Zugriff verweigert" fehl, wenn die Mitgliedschaft der SharePoint-Gruppe nicht auf jeder festgelegt ist.
  
 **Um dieses Problem zu beheben, führen Sie diese Schritte aus:**
  
 1. Erlauben Sie allen Mitgliedern der Mitglieder der SharePoint-Gruppe finden Sie unter. 
  
 2. Entfernen die SharePoint-Gruppe aus "an" oder "Cc" Zeile der e-Mail. 
  
 3. Die Benutzer explizit an oder CC hinzufügen auszurichten, wenn die Sichtbarkeit der Mitgliedschaft für SharePoint-Gruppe nicht geändert werden kann. 
  
Zum Anzeigen von finden Sie weitere Details auf [HTTP unbefugte zu /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

