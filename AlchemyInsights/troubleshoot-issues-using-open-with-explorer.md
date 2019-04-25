---
title: Behandeln von Problemen beim Öffnen mit Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390606"
---
# <a name="fix-problems-with-open-with-explorer"></a>Beheben von Problemen mit Open mit Explorer

Beheben häufig auftretender Probleme beim Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mit dem Befehl **Open with Explorer** : 
  
- Verwenden Sie Internet Explorer 10 oder Internet Explorer 11. **Open with Explorer** ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel. **Open with Explorer** ist in allen Browsern außer Internet Explorer deaktiviert. 
    
- **Open with Explorer** ist in der modernen Umgebung für SharePoint-Bibliotheken nicht verfügbar. Verwenden Sie stattdessen die **Ansicht im Datei-Explorer** . Wählen Sie **Ansichts Options** \> **Ansicht im Datei-Explorer**aus. Die Ansicht im Datei-Explorer ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel. **Ansicht im Datei-Explorer** in nur in Internet Explorer verfügbar. 
    
- Stellen Sie sicher, dass der webClient-Dienst gestartet wird. Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Option Desktop ausführen, geben Sie Services. msc ein, und drücken Sie dann die EINGABETASTE. Scrollen Sie nach unten zum webClient-Dienst, und stellen Sie sicher, dass in der Spalte **Status** die Option Running angezeigt wird. Wenn dies nicht der Fall ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. (Möglicherweise müssen Sie den Dienst zuerst aktivieren, indem Sie im Feld Starttyp **** entweder **manuell** oder **automatisch** auswählen.) 
    
> [!NOTE]
> Das Öffnen einer Bibliothek im Datei-Explorer ist praktisch, wenn Sie mehrere Dateien und Ordner einmal kopieren oder verschieben müssen, aber wenn Sie regelmäßig in der Bibliothek arbeiten möchten, wird die Synchronisierung empfohlen. Informationen zur Problembehandlung beim Öffnen im Datei-Explorer finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Weitere Informationen zum Einrichten der Synchronisierung finden Sie unter [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Weitere Informationen finden Sie im Artikel [Verwenden des Befehls "Öffnen mit Explorer" zur Behandlung von Problemen in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) . 
  

