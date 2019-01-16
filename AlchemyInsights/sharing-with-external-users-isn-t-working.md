---
title: Freigabe für externe Benutzer ist nicht funktionsfähig
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289811"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Beheben von Problemen, die gemeinsame Nutzung von SharePoint-Inhalten mit externen Benutzern

Stellen Sie sicher, dass externe Freigabe für Ihre Organisation aktiviert ist:
  
1. Wechseln Sie zu der [Services &amp; Seite im Office 365 Administrationscenter-add-ins](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), und klicken Sie auf **Sites**.
    
2. Stellen Sie sicher, dass die Einstellung auf "Aktiviert" aktiviert ist Wenn "Nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer in Office 365 Administrationscenter aufgeführt ist.
    
Stellen Sie sicher, dass externe Freigabe für die Website aktiviert. Für eine klassische Websitesammlung:
  
1. Klicken Sie in der klassischen SharePoint-Verwaltungskonsole im linken Bereich auf **Websitesammlungen**.
    
2. Wählen Sie die Website oder Websites, und klicken Sie auf dem Menüband auf **Freigabe**.
    
Für eine Teamwebsite, zu der eine Office 365-Gruppe gehört, oder eine Kommunikation-Website:
  
- Diese neuen Websitetypen haben die gleiche sharing festlegen als Ihrer Organisation geltende Einstellung, wenn die Einstellung der gesamten Organisation erlaubt die Freigabe von Dateien mithilfe von Links, die Anmeldung nicht erforderlich ist. In diesem Fall können die Websites mit neuen und vorhandenen externen Benutzern, die Anmeldung nutzt. Um die Einstellung für bestimmte Standorte zu ändern, verwenden Sie die neue SharePoint Administrationscenter (Preview) oder über PowerShell. [Erfahren Sie mehr](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Die externe Freigabe für jede Website können restriktiver als Ihrer Organisation geltende Einstellung, aber nicht mehr als die Einstellung der gesamten Organisation permissive festgelegt. 
  

