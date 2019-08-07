---
title: Suchen in SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059251"
---
# <a name="search-in-sharepoint-online"></a>Suchen in SharePoint Online

Inhalte müssen durchforstet und dem Suchindex hinzugefügt werden, damit Benutzer in SharePoint Online nach Ihren Suchvorgängen suchen können. Der Inhalt wird automatisch basierend auf einem vordefinierten durchforstungszeitplan gecrawlt (der durchforstungszeitplan kann nicht geändert werden). Der Crawler ruft Inhalte ab, die seit der letzten Durchforstung geändert wurden, und aktualisiert den Index. Wenn Sie sicherstellen möchten, dass Inhalt gecrawlt wird und der Index aktualisiert wird, beachten Sie Folgendes:

- Stellen Sie sicher, dass Inhalte gefunden werden können, indem [Websiteinhalte durchsuchbar gemacht](https://docs.microsoft.com/sharepoint/make-site-content-searchable)werden.

- Wenn Sie eine verwaltete Eigenschaft geändert oder die Zuordnung von durchforstete und verwalteten Eigenschaften geändert haben, muss die Website erneut durchforstet werden, bevor Ihre Änderungen im Suchindex wiedergegeben werden. 

    Da Ihre Änderungen im Suchschema und nicht auf der tatsächlichen Website vorgenommen werden, wird die Website vom Crawler nicht automatisch neu indiziert. 

    Weitere Informationen finden Sie unter [Manuelles anfordern der Durchforstung und erneuten Indizierung einer Website, einer Bibliothek oder einer Liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Warten Sie mindestens 24 Stunden nach der manuellen Anforderung einer Durchforstung und der vollständigen erneuten Indizierung, um zu sehen, ob noch ein Problem auftritt. 

    Wenn seit dem Initiieren der Durchforstung und der vollständigen erneuten Indizierung mehr als 24 Stunden vergangen sind, melden Sie sich einen Supportfall an. In vielen Fällen arbeiten wir bereits an einer Lösung. Geben Sie uns mindestens 24 Stunden, um eine Lösung zu vervollständigen.

>[! Wichtig!]: Wenn eine Website, ein Dokument (eine Bibliothek) oder eine Liste gelöscht wurde und weiterhin in den Suchergebnissen angezeigt wird, sollten Benutzer eine **Fehler 404-Datei** erhalten, die nicht gefunden wurde, wenn Sie versuchen, darauf zuzugreifen. Dieses Problem sollte bei weiteren Untersuchungen als Supportfall protokolliert werden. 



