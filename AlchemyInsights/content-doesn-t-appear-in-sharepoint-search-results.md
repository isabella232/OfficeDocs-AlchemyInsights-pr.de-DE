---
title: Inhalte werden nicht in SharePoint-Suchergebnissen angezeigt
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705660"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Inhalte werden nicht in SharePoint-Suchergebnissen angezeigt

Befolgen Sie diese Schritte zur Problembehandlung, wenn der erwartete Inhalt nicht in den Suchergebnissen angezeigt wird:
  
1. Stellen Sie sicher, dass die **Website** mit dem erwarteten Inhalt so festgelegt ist, dass Inhalte in den Suchergebnissen angezeigt werden können. Führen Sie die Schritte unter [Anzeigen von Inhalten auf einer Website in Suchergebnissen](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)aus.

2. Stellen Sie sicher, dass die **Liste** oder **Bibliothek** , die den erwarteten Inhalt enthält, so festgelegt ist, dass Inhalte in den Suchergebnissen angezeigt werden können. Führen Sie die Schritte unter [Anzeigen von Inhalten aus Listen oder Bibliotheken in Suchergebnissen aus](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Stellen Sie sicher, dass das Seiten-, Dokument-oder benutzerdefinierte Seitenlayout als **Hauptversion** veröffentlicht wird. Befolgen von Schritt 3 in der [Suche werden nicht alle Ergebnisse in SharePoint Online zurückgegeben](https://go.microsoft.com/fwlink/?linkid=874525).

4. Stellen Sie sicher, dass der Benutzer über **Berechtigungen** zum Anzeigen des Inhalts verfügt. Befolgen Sie die Schritte unter [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Wenn das Suchschema durch Hinzufügen einer neuen verwalteten Eigenschaft, durch Bearbeiten einer verwalteten Eigenschaft oder durch Entfernen einer verwalteten Eigenschaft geändert wurde, müssen Sie eine Durchforstung und eine erneute Indizierung anfordern. Führen Sie die Schritte unter [Manuelles anfordern des Durchforstens und erneuten Indizierens einer Website, einer Bibliothek oder einer Liste aus,](https://docs.microsoft.com/sharepoint/crawl-site-content)um den Inhalt **neu zu indizieren** . Dies kann eine Weile dauern, warten Sie 24 Stunden, bevor Sie die Ergebnisse erneut überprüfen.

Weitere Informationen finden Sie unter [Aktivieren des Inhalts einer Website, um durchsuchbar zu sein](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
