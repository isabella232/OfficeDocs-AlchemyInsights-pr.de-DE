---
title: Bereitstellen von Add-Ins für Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233524"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Bereitstellen von Add-Ins für Microsoft 365 Apps

Die zentrale Bereitstellung ist die empfohlene Methode zum Bereitstellen Office Add-Ins für Benutzer und Gruppen in Ihrer Organisation. Führen Sie zum Bereitstellen von Add-Ins die folgenden Schritte aus:

**Hinweis:** Informationen zum Installieren von Add-Ins für Office benutzer finden Sie unter [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d). Stellen Sie außerdem sicher, dass der individuelle Erwerb Office Store Add-Ins aktiviert ist. Weitere Informationen finden Sie unter [Prevent add-in downloads by off the Office Store across all clients (Except Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Stellen Sie sicher, dass Ihre Umgebung die Anforderungen für die Bereitstellung von Add-Ins mithilfe der zentralisierten Bereitstellung erfüllt. Weitere Informationen finden Sie unter [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Wechseln Sie **zu Einstellungen** Integrierte Apps Apps im Microsoft 365 Admin Center zum Bereitstellen  >    >   von Add-Ins. 

Hinweise: 

- Integrierte Apps erfordern, dass der Administrator über globale Administrator- oder Exchange Administratorberechtigungen verfügt.

- Bei der Bereitstellung von Add-Ins für mehrere Benutzer wird empfohlen, Zuweisungen mithilfe von Gruppen anstelle einzelner Benutzer zu erstellen. Weitere Informationen finden Sie unter [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- Die zentrale Bereitstellung unterstützt keine Benutzer in geschachtelten Gruppen oder Gruppen mit übergeordneten Gruppen. Weitere Informationen finden Sie unter [Benutzer- und Gruppenzuweisungen](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Stellen Sie sicher, dass der Microsoft 365-App-Verwaltungsdienst (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') für die Anmeldung aktiviert ist. Weitere Informationen finden Sie unter [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Wenn Probleme beim Bereitstellen von Add-Ins mithilfe von integrierten Apps auftreten, versuchen Sie, die Bereitstellung mithilfe von [Add-Ins zu versuchen.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Weitere Informationen finden Sie unter:

[Bereitstellen von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Verwalten von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Verwenden der PowerShell-Cmdlets für die zentrale Bereitstellung zum Verwalten von Add-Ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Veröffentlichen Office Add-Ins mithilfe der zentralen Bereitstellung über](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) das Microsoft 365 Admin Center 
 [Problembehandlung: Benutzer sieht keine Add-Ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Behandeln von Benutzerfehlern mit Office-Add-Ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)