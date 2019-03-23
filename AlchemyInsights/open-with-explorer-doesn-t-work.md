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
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764907"
---
# <a name="open-with-explorer-isnt-working"></a>Mit Explorer öffnen funktioniert nicht

Wenn **mit Explorer** oder **Ansicht im Datei-Explorer** öffnen nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst **ausgeführt** wird, indem Sie die folgenden Schritte ausführen. Beispielsweise kann es sehr viel Zeit in Anspruch nehmen, eine SharePoint-oder OneDrive-Bibliothek zu öffnen, wenn der Dienst nicht ausgeführt wird. 
  
1. Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Option Desktop ausführen aus, geben Sie Services. msc ein, und drücken Sie die **EINGABETASTE**.
    
2. Scrollen Sie nach unten zum webClient-Dienst, und überprüfen Sie die Spalte **Status** . Wenn der webClient-Dienststatus nicht **aktiv**ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. Aktivieren Sie den Dienst, falls erforderlich, indem Sie im Feld Starttyp entweder **** **manuell** oder **automatisch** auswählen. 
    
> [!NOTE]
> Informationen zur Problembehandlung beim Öffnen im Datei-Explorer finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). UnterSuchen Sie die Synchronisierung als bessere Alternative: [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

