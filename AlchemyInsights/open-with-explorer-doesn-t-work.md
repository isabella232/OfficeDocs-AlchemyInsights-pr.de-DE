---
title: "\"Mit Explorer öffnen\" funktioniert nicht"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694455"
---
# <a name="open-with-explorer-isnt-working"></a>Öffnen mit Explorer ist nicht funktionsfähig

Wenn **Open with Explorer** oder **View im Datei-Explorer** nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst auf " **Running** " festgelegt ist, indem Sie die folgenden Schritte ausführen. Es kann beispielsweise eine lange Zeit dauern, eine SharePoint-oder OneDrive-Bibliothek zu öffnen, wenn der Dienst nicht ausgeführt wird. 
  
1. Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Desktop-App ausführen aus, geben Sie Services. msc ein, und drücken Sie die **EINGABETASTE**.
    
2. Scrollen Sie nach unten zum WebClient Dienst, und überprüfen Sie die Spalte **Status** . Wenn der WebClient-Dienststatus nicht **aktiv**ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. Aktivieren Sie den Dienst, falls erforderlich, indem Sie im Feld **Starttyp** entweder **manuell** oder **automatisch** auswählen. 
    
> [!NOTE]
> Informationen zum Behandeln von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Durchsuchen Sie die Synchronisierung als bessere Alternative: [Synchronisieren Sie SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

