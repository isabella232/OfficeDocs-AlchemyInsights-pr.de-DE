---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758730"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Gruppe mit verbundener Website in SharePoint Online erstellen

Beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen sind einige häufige Probleme aufgetreten.

 Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.

Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter [Erste Schritte mit SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell aus gelöschten Websites.

Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten, dass bereits eine andere Gruppe mit demselben Alias vorhanden ist, überprüfen Sie die vorhandenen Gruppen aus dem [Office 365 aus dem Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.

Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.

Sie können vorhandene Websites mit einer Office 365 Gruppe verbinden. Weitere Informationen finden Sie unter [Verbinden einer Office 365 Gruppe mit dem SharePoint-Benutzer ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Um eine verbundene Website mit Office 365 Gruppe zu erstellen, müssen Sie eine Team Website erstellen. Weitere Informationen finden Sie unter [Erstellen einer Teamwebsite in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

