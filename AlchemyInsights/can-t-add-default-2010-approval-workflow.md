---
title: Kann nicht hinzugefügt werden Standard 2010 Genehmigungsworkflow (engl.)
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469561"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Kann nicht hinzugefügt werden Standard 2010 Genehmigungsworkflow (engl.)

Sie können nicht in einer Microsoft SharePoint-Websitesammlung ein Global wieder verwendbaren Workflows (beispielsweise "Genehmigung - SharePoint 2010") zu einer Liste oder Bibliothek hinzufügen.
  
Gehen Sie folgendermaßen vor, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Standortobjekten** **Workflows**aus. 
  
3. Wählen Sie im Abschnitt **neu** des Menübands **Workflows** **Wieder Verwendbarer Workflow**aus. 
  
4. Klicken Sie auf das Formular **Wieder verwendbaren Workflow erstellen** , geben Sie den Namen * **Repair2010***. Wählen Sie für **Plattformtyp** **SharePoint 2010-Workflow**aus, und wählen Sie dann auf **OK**. 
  
5. Aktivieren Sie im Abschnitt **Speichern** des Menübands **Workflow** **Veröffentlichen**. 
  
6. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** **Global veröffentlichen**. Klicken Sie im Dialogfeld Bestätigung wählen Sie **OK**aus. 
  
7. In einem Webbrowser die Stammwebsite der Websitesammlung zu suchen, und klicken Sie dann auf zugreifen **Site Settings** \> **Websitesammlungs-Features**. Klicken Sie dann Umschalten des **Workflows** Features: 
  
· Wenn das Feature *aktiviert* ist, klicken Sie auf **deaktivieren,** und klicken Sie dann auf **Aktivieren**. 
  
· Wenn das Feature *deaktiviert* ist, klicken Sie auf **Aktivieren**. 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

