---
title: 2010-Genehmigungs Workflow kann nicht hinzugefügt werden
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366834"
---
# <a name="unable-to-add-2010-approval-workflow"></a>2010-Genehmigungs Workflow kann nicht hinzugefügt werden

In einer Microsoft SharePoint-Websitesammlung können Sie einer Liste oder Bibliothek keinen Global wiederverwendbaren Workflow (wie "Genehmigungs-SharePoint 2010") hinzufügen.
  
Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Website Objekte**die Option **Workflows**aus. 
  
3. Wählen Sie im Abschnitt **neu** des Menübands **Workflows** **wieder verwendbarer Workflow**aus. 
  
4. Geben Sie im Formular **wieder verwendbare Workflows erstellen** den Namen * * *Repair2010* * * ein. Klicken Sie unter **Plattformtyp**auf **sharePoint 2010-Workflow**, und klicken Sie dann auf **OK**. 
  
1. Wählen Sie im **Workflow** -Menüband im Abschnitt **Speichern** die Option **veröffentlichen**aus. 
  
2. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** die Option **Global veröffentlichen**aus. Klicken Sie im daraufhin angezeigten Bestätigungsdialogfeld auf **OK**. 
  
3. Navigieren Sie in einem Webbrowser zu der Stammwebsite der Websitesammlung, und greifen Sie dann auf Website **Sammlungs Features**für **Websiteeinstellungen** \> zu. UmSchalten des **Workflows** -Features: 
  
· Wenn das Feature *aktiviert* ist, klicken Sie auf Deaktivieren **,** und klicken Sie dann auf **aktivieren**. 
  
· Wenn das Feature *deaktiviert* ist, klicken Sie auf **aktivieren**. 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

