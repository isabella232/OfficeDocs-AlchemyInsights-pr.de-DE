---
title: Gewähren von Benutzern Zugriff auf SharePoint und OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d29764266f44aee5f8f8e2c93ad67b2a33c6f417
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/22/2019
ms.locfileid: "30209736"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Gewähren von Benutzern Zugriff auf SharePoint und OneDrive

> [!NOTE]
> Wenn ein OneDrive oder eine SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein temporäres Dienst Problem vorliegen. [Überprüfen des Dienststatus](https://portal.office.com/adminportal/home#/servicehealth) -Dashboards
  
Wenn Sie möchten, dass Personen in Ihrer Organisation sich anmelden und SharePoint und OneDrive verwenden können, müssen Sie diese Konten hinzufügen und sicherstellen, dass Sie über eine Lizenz verfügen, die Ihnen Zugriff auf SharePoint und OneDrive ermöglicht. Die einfachste Möglichkeit zum Hinzufügen von Benutzern befindet sich im Microsoft 365 Admin Center.
  
1. Wechseln Sie zur [Seite aktive Benutzer im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/users), und klicken Sie dann auf **Benutzer hinzufügen**.
    
2. Geben Sie die Informationen für den Benutzer ein, und stellen Sie sicher, dass unter **Produktlizenzen**eine Lizenz zugewiesen und **SharePoint Online** ausgewählt ist. 
    
Beachten Sie, dass, wenn Sie die externe Freigabe in Ihrer Organisation zulassen, Benutzer SharePoint-und OneDrive-Inhalte für Personen außerhalb der Organisation freigeben können. Sie müssen diese externen Benutzerlizenzen nicht erteilen. Sie müssen auch keine Konten für Sie hinzufügen, es sei denn, die Freigabe ist auf "nur vorhandene externe Benutzer" festgelegt. Wenn die Personen in diesem Fall nicht im Verzeichnis Ihrer Organisation sind, müssen Sie diese als Gastbenutzer im Azure AD Admin Center hinzufügen.
  

