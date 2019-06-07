---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759080"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

Es gibt viele Möglichkeiten, den Zugriff auf SharePoint Online/OneDrive-Dienste einzuschränken. Diese verschiedenen Methoden zur Zugriffseinschränkung werden weiter unten beschrieben. 

Berechtigungs Beschränkung

In SharePoint Online und OneDrive für Unternehmen beschränken wir den Zugriff auf Elemente wie Websites, Dateien und Ordner, indem wir nur Zugriff auf diese Gruppen/Personen gewähren, die Zugriff haben sollten.

[Anpassen von Berechtigungen für eine SharePoint-Liste oder-Bibliothek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Anpassen von SharePoint-Websiteberechtigungen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[Ändern der Berechtigungen für einen Unterordner](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Steuern des Zugriffs von nicht verwalteten Geräten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als SharePoint-oder globaler Administrator in Office 365 können Sie den Zugriff auf SharePoint-und OneDrive-Inhalte von nicht verwalteten Geräten (die nicht mit Hybrid-AD verbunden oder in InTune kompatibel sind) blockieren oder einschränken.

Einschränkung des Netzwerkstandorts

Als IT-Administrator können Sie den Zugriff auf SharePoint-und OneDrive-Ressourcen basierend auf definierten Netzwerkstandorten steuern, denen Sie vertrauen. Dies wird auch als standortbasierte Richtlinie bezeichnet. Weitere Informationen finden Sie unter [Steuern des Zugriffs auf SharePoint Online-und OneDrive-Daten basierend auf dem Netzwerkstandort](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .

Einschränkung der Website Sperre 

In SharePoint Online haben Sie die Möglichkeit, eine Websitesammlung zu sperren, sodass niemand Zugriff hat. Dies wird über PowerShell und die [SharePoint Online-Verwaltungsshell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) mithilfe der Eigenschaft " [Sets-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState" festgelegt.

Einschränken der Benutzer am Erstellen von Websites oder Unterwebsites

Als SharePoint-Administrator oder Office 365 globaler Administrator können Sie Ihren Benutzern die Erstellung und Verwaltung Ihrer eigenen SharePoint-Websites ermöglichen, bestimmen, welche Art von Websites Sie erstellen können, und den Speicherort der Websites angeben. Weitere Informationen finden Sie unter [Manage Site Creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

