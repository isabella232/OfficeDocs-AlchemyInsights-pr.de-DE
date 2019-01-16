---
title: Kann nicht für einen Genehmigungsworkflow 2010 hinzugefügt werden
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290266"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Kann nicht für einen Genehmigungsworkflow 2010 hinzugefügt werden

Sie können nicht in einer Microsoft SharePoint-Websitesammlung ein Global wieder verwendbaren Workflows (beispielsweise "Genehmigung - SharePoint 2010") zu einer Liste oder Bibliothek hinzufügen.
  
Gehen Sie folgendermaßen vor, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Standortobjekten** **Workflows**aus. 
  
3. Wählen Sie im Abschnitt **neu** des Menübands **Workflows** **Wieder Verwendbarer Workflow**aus. 
  
4. Klicken Sie auf das Formular **Wieder verwendbaren Workflow erstellen** , geben Sie den Namen ** *Repair2010* **. Klicken Sie auf **SharePoint 2010-Workflows**für **Plattformtyp**und klicken Sie dann auf **OK**. 
  
1. Aktivieren Sie im Abschnitt **Speichern** des Menübands **Workflow** **Veröffentlichen**. 
  
2. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** **Global veröffentlichen**. Klicken Sie im Dialogfeld Bestätigung wählen Sie **OK**aus. 
  
3. In einem Webbrowser die Stammwebsite der Websitesammlung zu suchen, und klicken Sie dann auf zugreifen **Site Settings** \> **Websitesammlungs-Features**. Schalten Sie das Feature **Workflows** : 
  
· Wenn das Feature *aktiviert* ist, klicken Sie auf **deaktivieren,** und klicken Sie dann auf **Aktivieren**. 
  
· Wenn das Feature *deaktiviert* ist, klicken Sie auf **Aktivieren**. 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

