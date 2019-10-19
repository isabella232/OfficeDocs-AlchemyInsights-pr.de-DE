---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750519"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Probleme beim Erstellen oder gruppieren verbundener Websites in SharePoint Online

Beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen sind einige häufige Probleme aufgetreten.

 Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.

Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites.

Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten, dass bereits eine andere Gruppe mit demselben Alias vorhanden ist, überprüfen Sie die vorhandenen Gruppen aus dem [Office 365 aus dem Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.

Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.

Sie können vorhandene Websites mit einer Office 365 Gruppe verbinden. Weitere Informationen finden Sie unter [Verbinden einer Office 365 Gruppe mit dem SharePoint-Benutzer ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Um eine verbundene Website mit Office 365 Gruppe zu erstellen, müssen Sie eine Team Website erstellen. Weitere Informationen finden Sie unter [Erstellen einer Teamwebsite in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

