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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719481"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Gruppe mit verbundener Website in SharePoint Online erstellen

<p><strong>Beim Erstellen oder erneuten Erstellen einer verbundenen Website mit Gruppen sind einige häufige Probleme aufgetreten.&nbsp;</strong></p>  <p>1.Wenn Sie eine Gruppe und die verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.</p>  <ul>  <li>Download <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO-Verwaltungsshell</a> - Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie <a title="unter Erste Schritte mit SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Erste Schritte mit SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Entfernen der Website aus gelöschten Websites mithilfe <a title="der Remove-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remove-SPODeletedSite</a> PowerShell-Cmdlet.</li>  </ul>  <p>Wenn Sie eine verbundene Website mit einer Gruppe erstellen und eine Warnung erhalten, dass <strong>"eine andere Gruppe mit demselben Alias bereits vorhanden ist"</strong>, überprüfen <a title="Sie die vorhandenen Gruppen aus dem Office 365 aus dem Admin Center." href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 aus dem Admin Center</a>. Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn Sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias zugewiesen.&nbsp;</p>  <p><strong>Es gibt verschiedene Möglichkeiten, um moderne Gruppen mit SharePoint zu erstellen und zu verwenden.&nbsp;</strong></p>  <ol>  <li>Sie können vorhandene Websites mit einer Office 365 Gruppe verbinden. Weitere Informationen finden Sie unter <a title="Verbinden einer Office 365 Gruppe mit dem SharePoint-Benutzer ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Verbinden einer Office 365 Gruppe mit dem SharePoint-</a>Benutzer ineterface.</li>  <li>Um eine verbundene Website mit Office 365 Gruppe zu erstellen, müssen Sie eine Team Website erstellen. Weitere Informationen finden Sie unter <a title="Erstellen einer Teamwebsite in SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Erstellen Sie eine Teamwebsite in SharePoint.</a></li>  </ol>

