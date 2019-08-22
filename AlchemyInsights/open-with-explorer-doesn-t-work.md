---
title: "\"Mit Explorer öffnen\" funktioniert nicht"
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
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538469"
---
# <a name="open-with-explorer-isnt-working"></a>Öffnen mit Explorer ist nicht funktionsfähig

Wenn **Open with Explorer** oder **View im Datei-Explorer** nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst auf " **Running** " festgelegt ist, indem Sie die folgenden Schritte ausführen. Es kann beispielsweise eine lange Zeit dauern, eine SharePoint-oder OneDrive-Bibliothek zu öffnen, wenn der Dienst nicht ausgeführt wird. 
  
1. Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Desktop-App ausführen aus, geben Sie Services. msc ein, und drücken Sie die **EINGABETASTE**.
    
2. Scrollen Sie nach unten zum WebClient Dienst, und überprüfen Sie die Spalte **Status** . Wenn der WebClient-Dienststatus nicht **aktiv**ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. Aktivieren Sie den Dienst, falls erforderlich, indem Sie im Feld Starttyp entweder **** **manuell** oder **automatisch** auswählen. 
    
> [!NOTE]
> Informationen zum Behandeln von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Durchsuchen Sie die Synchronisierung als bessere Alternative: [Synchronisieren Sie SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

