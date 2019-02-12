---
title: Mit Explorer öffnen funktioniert nicht
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906803"
---
# <a name="open-with-explorer-isnt-working"></a>Mit Explorer öffnen ist nicht funktionsfähig

Falls **mit Explorer öffnen** oder **im Datei-Explorer-Ansicht** nicht funktioniert stellen Sie sicher, dass der WebClient-Dienst **ausgeführt** wird durch die folgenden Schritte. Beispielsweise könnte dauert lange, bis eine Bibliothek für SharePoint oder OneDrive geöffnet wird, wenn der Dienst nicht ausgeführt wird. 
  
1. Klicken Sie im Suchfeld Windows Typ ausführen, wählen Sie ausführen-desktop-app, geben Sie Services.msc ein, und wählen Sie dann **EINGABETASTE**.
    
2. Führen Sie einen Bildlauf nach unten zu den WebClient-Dienst, und überprüfen Sie die Spalte **Status** . Ist der Status der WebClient-Dienst nicht **ausgeführt wird**, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. Aktivieren Sie den Dienst bei Bedarf, indem Sie in **der Liste Starttyp** **manuell** oder **automatisch** auswählen. 
    
> [!NOTE]
> Zum Beheben von Startproblemen im Datei-Explorer öffnen finden Sie unter [im Explorer öffnen](https://go.microsoft.com/fwlink/?linkid=871665). Erkunden Sie die Synchronisierung als bessere Alternative: [Synchronisierung SharePoint-Dateien mit der neuen OneDrive Sync-Client](https://go.microsoft.com/fwlink/?linkid=871666). 
  

