---
title: 2010-Genehmigungs Workflow kann nicht hinzugefügt werden
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699734"
---
# <a name="unable-to-add-2010-approval-workflow"></a>2010-Genehmigungs Workflow kann nicht hinzugefügt werden

In einer Microsoft SharePoint-Websitesammlung können Sie einer Liste oder Bibliothek keinen Global wiederverwendbaren Workflow (beispielsweise "Genehmigungs SharePoint 2010") hinzufügen.
  
Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Website Objekte**die Option **Workflows**aus. 
  
3. Wählen Sie im **neuen** Abschnitt des Menübands **Workflows** die Option **wieder verwendbarer Workflow**aus. 
  
4. Geben Sie im Formular **wiederverwendbaren Workflow erstellen** den Namen * * *Repair2010* * * ein. Klicken Sie unter **Plattformtyp**auf **SharePoint 2010 Workflow**, und klicken Sie dann auf **OK**. 
  
1. Wählen Sie im Abschnitt **Speichern** des Menübands **Workflow** die Option **veröffentlichen**aus. 
  
2. Wählen Sie im Abschnitt **Manage** des Menübands **Workflow** die Option **Global veröffentlichen**aus. Wählen Sie im daraufhin angezeigten Dialogfeld Bestätigung die Option **OK**aus. 
  
3. Suchen Sie in einem Webbrowser die Stammwebsite der Websitesammlung, und greifen Sie dann auf **Site Settings** Website \> **Sammlungs Features**für Websiteeinstellungen zu. Umschalten des **Workflows** -Features: 
  
· Wenn das Feature  *aktiviert*  ist, klicken Sie auf Deaktivieren **,** und klicken Sie dann auf **aktivieren**. 
  
· Wenn das Feature  *deaktiviert*  ist, klicken Sie auf **aktivieren**. 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

