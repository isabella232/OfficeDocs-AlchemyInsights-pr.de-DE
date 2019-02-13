---
title: Beheben von Problemen beim Öffnen mit Explorer verwenden
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 9b2abe01a47d39812988d62b6f010a8933fad33e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929203"
---
# <a name="fix-problems-with-open-with-explorer"></a>Beheben von Problemen mit mit Explorer öffnen

Beheben von Problemen mit dem Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mit dem Befehl **mit Explorer öffnen** : 
  
- Verwenden Sie InternetExplorer 10 oder InternetExplorer 11. **Mit Explorer öffnen** ist nicht kompatibel mit Microsoft Edge, Google Chrome, Firefox und andere Personen. **Mit Explorer öffnen** ist in allen Browsern außer Internet Explorer deaktiviert. 
    
- **Mit Explorer öffnen** ist nicht verfügbar, moderne Oberfläche für SharePoint-Bibliotheken. Verwenden Sie stattdessen die **Ansicht im Datei-Explorer** . Wählen Sie die **Ansichtsoptionen** \> **Ansicht im Datei-Explorer**. Ansicht im Datei-Explorer ist nicht kompatibel mit Microsoft Edge, Google Chrome, Firefox und andere Personen. **Ansicht im Datei-Explorer** in nur in Internet Explorer verfügbar. 
    
- Stellen Sie sicher, dass der WebClient-Dienst ausgeführt wird. Wählen Sie im Suchfeld Windows Typ ausgeführt werden soll die Run-desktop-app, geben Sie Services.msc ein, und drücken Sie die EINGABETASTE. Führen Sie einen Bildlauf nach unten zu den WebClient-Dienst, und stellen Sie sicher, dass die Spalte **Status** angezeigt werden "Ausführen". Wenn dies nicht der Fall, doppelklicken Sie auf den Dienst, klicken Sie auf **Start**, und klicken Sie dann auf **OK**. (Möglicherweise müssen Sie zunächst den Dienst aktivieren, indem Sie entweder **manuell** oder **automatisch** in das Feld **Starttyp** auswählen.) 
    
> [!NOTE]
> Öffnen einer Dokumentbibliothek im Datei-Explorer ist hilfreich, wenn Sie kopieren oder verschieben Sie mehrere Dateien und Ordner nach, jedoch sollten Sie regelmäßig in der Bibliothek arbeiten müssen, wird empfohlen, synchronisieren es. Zum Beheben von Startproblemen im Datei-Explorer öffnen finden Sie unter [im Explorer öffnen](https://go.microsoft.com/fwlink/?linkid=871665). Info zum Einrichten von Sync finden Sie unter [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-Synchronisierungsclient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Finden Sie weitere Informationen im Artikel [zum Verwenden des Befehls "mit Explorer öffnen" zum Behandeln von Problemen in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) . 
  

