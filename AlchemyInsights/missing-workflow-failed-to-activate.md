---
title: Fehlender Workflow konnte nicht aktiviert werden
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753795"
---
# <a name="missing-workflow-failed-to-activate"></a>Fehlender Workflow konnte nicht aktiviert werden

In einer Microsoft SharePoint-Websitesammlung können Sie einer Liste oder Bibliothek keinen Global wiederverwendbaren Workflow (beispielsweise "Genehmigungs SharePoint 2010") hinzufügen.
  
Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Website Objekte**die Option **Workflows**aus. 
  
3. Wählen Sie im **neuen** Abschnitt des Menübands **Workflows** die Option **wieder verwendbarer Workflow**aus. 
  
4. Geben Sie im Formular **wiederverwendbaren Workflow erstellen** den Namen * * *Repair2010* * * ein. Klicken Sie unter **Plattformtyp**auf **SharePoint 2010 Workflow**, und klicken Sie dann auf **OK**. 
  
1. Wählen Sie im Abschnitt **Speichern** des Menübands **Workflow** die Option **veröffentlichen**aus. 
  
2. Wählen Sie im Abschnitt **Manage** des Menübands **Workflow** die Option **Global veröffentlichen**aus. Wählen Sie im daraufhin angezeigten Dialogfeld Bestätigung die Option **OK**aus. 
  
3. Suchen Sie in einem Webbrowser die Stammwebsite der Websitesammlung, und greifen Sie dann auf Website **Sammlungs Features**für **Websiteeinstellungen** \> zu. Aktivieren Sie dann das Feature **Workflows** : 
  
· Wenn das Feature *aktiviert* ist, klicken Sie auf Deaktivieren **,** und klicken Sie dann auf **aktivieren**. 
  
· Wenn das Feature *deaktiviert* ist, klicken Sie auf **aktivieren**. 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

