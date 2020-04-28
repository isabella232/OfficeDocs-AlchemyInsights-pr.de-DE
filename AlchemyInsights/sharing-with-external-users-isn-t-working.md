---
title: Die Freigabe für externe Benutzer funktioniert nicht
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913001"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Beheben von Problemen beim Freigeben von SharePoint-Inhalten mit externen Benutzern

Stellen Sie sicher, dass die externe Freigabe für Ihre Organisation aktiviert ist:
  
1. Wechseln Sie zur [Seite &amp; Dienste-Add-Ins im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), und klicken Sie auf **Websites**.
    
2. Stellen Sie sicher, dass die Einstellung auf "ein" aktiviert ist. Wenn "nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer im Microsoft 365 Admin Center aufgeführt ist.
    
Stellen Sie sicher, dass die externe Freigabe für die Website aktiviert wurde. Für eine klassische Websitesammlung:
  
1. Klicken Sie im neuen SharePoint Admin Center im linken Bereich auf **Websites**.
    
2. Wählen Sie die Website oder Standorte aus, und klicken Sie auf dem Menüband auf **Freigabe**.
    
Für eine Teamwebsite, die zu einer Microsoft 365-Gruppe oder einer Kommunikationswebsite gehört:
  
- Diese neuen Websitetypen weisen dieselbe Freigabe Einstellung wie Ihre organisationsweite Einstellung auf, es sei denn, die Einstellung für die gesamte Organisation ermöglicht das Freigeben von Dateien über Links, die keine Anmeldung erfordern. In diesem Fall können die Websites die Freigabe für neue und vorhandene externe Benutzer zulassen, die sich anmelden. Um die Einstellung für bestimmte Websites zu ändern, verwenden Sie das neue SharePoint Admin Center oder PowerShell. [Weitere Informationen](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Die Einstellung für die externe Freigabe für jeden Standort kann restriktiver sein als die organisationsweite Einstellung, jedoch nicht restriktiver als die organisationsweite Einstellung. 
  

