---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771200"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleme beim Erstellen einer mit einer Gruppe verbundenen Website in SharePoint

1. Einige häufige Probleme, die beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen auftreten.
Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.

   - Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites. PowerShell ist erforderlich, um Gruppen Websites endgültig zu löschen.

1. Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten: **bereits eine andere Gruppe mit demselben Alias vorhanden**ist, überprüfen Sie die vorhandenen Gruppen im [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.

1. Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.

   - Sie können vorhandene Websites mit einer Microsoft 365-Gruppe verbinden. Weitere Informationen finden Sie unter [Verbinden einer Microsoft 365-Gruppe mithilfe der SharePoint-Benutzeroberfläche](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Um eine verbundene Website der Microsoft 365-Gruppe zu erstellen, müssen Sie eine [Team Website](https://admin.microsoft.com/sharepoint)erstellen.
