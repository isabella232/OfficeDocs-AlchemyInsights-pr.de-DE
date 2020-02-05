---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770350"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleme beim Erstellen einer mit einer Gruppe verbundenen Website in SharePoint

1. Einige häufige Probleme, die beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen auftreten.
Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.

   - Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites. PowerShell ist erforderlich, um Gruppen Websites endgültig zu löschen.

1. Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten: **bereits eine andere Gruppe mit demselben Alias vorhanden**ist, überprüfen Sie die vorhandenen Gruppen aus dem [Office 365 aus dem Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.

1. Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.

   - Sie können vorhandene Websites mit einer Office 365 Gruppe verbinden. Weitere Informationen finden Sie unter [Verbinden einer Office 365 Gruppe mithilfe der SharePoint-Benutzeroberfläche](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Um eine verbundene Website mit Office 365 Gruppe zu erstellen, müssen Sie eine [Team Website](https://admin.microsoft.com/sharepoint)erstellen.
