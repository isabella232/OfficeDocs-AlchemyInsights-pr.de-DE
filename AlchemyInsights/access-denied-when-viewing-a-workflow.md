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
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883590"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff verweigert beim Anzeigen eines Workflows

SharePoint 2013 Workflows, die versuchen, eine e-Mail an eine SharePoint-Gruppe zu senden, können mit der Fehlermeldung "Zugriff verweigert" fehlschlagen, wenn die Mitgliedschaft in der SharePoint-Gruppe nicht auf jeder festgelegt ist.
  
 **Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**
  
 1. Lassen Sie alle Mitglieder der SharePoint-Gruppe anzeigen.
  
 2. Entfernen Sie die SharePoint-Gruppe aus der an-oder CC-Zeile der e-Mail.
  
 3. Fügen Sie die Benutzer explizit zur Zeile "an" oder "CC" hinzu, wenn die Mitgliedschafts Sichtbarkeit für SharePoint-Gruppe nicht geändert werden kann.
  
Weitere Informationen finden Sie unter [http Unauthorized to/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  