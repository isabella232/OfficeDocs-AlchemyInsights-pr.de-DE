---
title: Freigabe für externe Benutzer funktioniert nicht
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207684"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Beheben von Problemen beim Freigeben von SharePoint-Inhalten für externe Benutzer

Stellen Sie sicher, dass die externe Freigabe für Ihre Organisation aktiviert ist:
  
1. Wechseln Sie zur [Seite &amp; Dienste-Add-ins im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), und klicken Sie auf **Websites**.
    
2. Stellen Sie sicher, dass die Einstellung auf "ein" aktiviert ist. Wenn "nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer im Microsoft 365 Admin Center aufgeführt ist.
    
Stellen Sie sicher, dass die externe Freigabe für die Website aktiviert ist. Für eine klassische Websitesammlung:
  
1. Klicken Sie im klassischen SharePoint Admin Center im linken Bereich auf **Websitesammlungen**.
    
2. Wählen Sie die Website oder Websites aus, und klicken Sie auf dem Menüband auf **Freigabe**.
    
Für eine Teamwebsite, die zu einer Office 365-Gruppe oder einer Kommunikationswebsite gehört:
  
- Diese neuen Websitetypen haben dieselbe Freigabe Einstellung wie Ihre organisationsweite Einstellung, es sei denn, die organisationsweite Einstellung ermöglicht das Freigeben von Dateien mit Links, die keine Anmeldung erfordern. In diesem Fall ermöglichen die Websites die Freigabe für neue und vorhandene externe Benutzer, die sich anmelden. Um die Einstellung für bestimmte Websites zu ändern, verwenden Sie das neue SharePoint Admin Center (Preview) oder PowerShell. [Weitere Informationen](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Die Einstellung für die externe Freigabe für jede Website kann restriktiver sein als die organisationsweite Einstellung, aber nicht mehr als die organisationsweite Einstellung. 
  

