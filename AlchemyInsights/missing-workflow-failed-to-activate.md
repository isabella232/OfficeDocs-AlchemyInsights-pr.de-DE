---
title: Fehlende Workflow konnte nicht aktiviert
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917567"
---
# <a name="missing-workflow-failed-to-activate"></a>Fehlende Workflow konnte nicht aktiviert

Sie können nicht in einer Microsoft SharePoint-Websitesammlung ein Global wieder verwendbaren Workflows (beispielsweise "Genehmigung - SharePoint 2010") zu einer Liste oder Bibliothek hinzufügen.
  
Gehen Sie folgendermaßen vor, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Standortobjekten** **Workflows**aus. 
  
3. Wählen Sie im Abschnitt **neu** des Menübands **Workflows** **Wieder Verwendbarer Workflow**aus. 
  
4. Klicken Sie auf das Formular **Wieder verwendbaren Workflow erstellen** , geben Sie den Namen ** *Repair2010* **. Klicken Sie auf **SharePoint 2010-Workflows**für **Plattformtyp**und klicken Sie dann auf **OK**. 
  
1. Aktivieren Sie im Abschnitt **Speichern** des Menübands **Workflow** **Veröffentlichen**. 
  
2. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** **Global veröffentlichen**. Klicken Sie im Dialogfeld Bestätigung wählen Sie **OK**aus. 
  
3. In einem Webbrowser die Stammwebsite der Websitesammlung zu suchen, und klicken Sie dann auf zugreifen **Site Settings** \> **Websitesammlungs-Features**. Klicken Sie dann Umschalten des **Workflows** Features: 
  
· Wenn das Feature *aktiviert* ist, klicken Sie auf **deaktivieren,** und klicken Sie dann auf **Aktivieren**. 
  
· Wenn das Feature *deaktiviert* ist, klicken Sie auf **Aktivieren**. 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

