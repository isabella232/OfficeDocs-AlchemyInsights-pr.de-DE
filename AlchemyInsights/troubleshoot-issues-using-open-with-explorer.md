---
title: Behandeln von Problemen mit "Öffnen mit Explorer"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659057"
---
# <a name="fix-problems-with-open-with-explorer"></a>Beheben von Problemen mit dem Öffnen mit dem Explorer

Beheben Sie häufige Probleme beim Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mit dem Befehl **Öffnen mit Explorer** : 
  
- Verwenden Sie Internet Explorer 10 oder Internet Explorer 11. **Open with Explorer** ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel. **Mit Explorer öffnen** ist in allen Browsern außer Internet Explorer deaktiviert. 
    
- **Open with Explorer** steht in der modernen Benutzeroberfläche für SharePoint-Bibliotheken nicht zur Verfügung. Verwenden Sie stattdessen die **Ansicht im Datei-Explorer** . Wählen Sie Ansichts **Optionen** \> **anzeigen im Datei-Explorer**aus. Die Ansicht im Datei-Explorer ist nicht mit Microsoft Edge, Google Chrome, Firefox und anderen kompatibel. Im **Datei-Explorer anzeigen** nur in Internet Explorer verfügbar. 
    
- Stellen Sie sicher, dass der WebClient-Dienst aktiv ist. Geben Sie im Feld Windows-Suche ausführen ein, wählen Sie die Option Desktop-App ausführen aus, geben Sie Services. msc ein, und drücken Sie dann die EINGABETASTE. Scrollen Sie nach unten zum WebClient Dienst, und stellen Sie sicher, dass in der Spalte **Status** die Meldung "Running" angezeigt wird. Wenn dies nicht der Fall ist, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. (Möglicherweise müssen Sie den Dienst zunächst aktivieren, indem Sie im Feld **Starttyp** entweder **manuell** oder **automatisch** auswählen.) 
    
> [!NOTE]
> Das Öffnen einer Bibliothek im Datei-Explorer ist praktisch, wenn Sie mehrere Dateien und Ordner einmal kopieren oder umlegen müssen, aber wenn Sie regelmäßig in der Bibliothek arbeiten möchten, empfehlen wir die Synchronisierung. Informationen zum Behandeln von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Informationen zum Einrichten der Synchronisierung finden Sie unter [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Weitere Informationen finden Sie im Artikel [Verwenden des Befehls "Open with Explorer" zur Behandlung von Problemen in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

