---
title: Suchen in SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507630"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Durchforsten und Indizieren von Inhalten in SharePoint Online

Inhalte müssen durchforstet und dem Suchindex hinzugefügt werden, damit Benutzer in SharePoint Online nach Ihren Suchvorgängen suchen können. Der Inhalt wird automatisch basierend auf einem vordefinierten durchforstungszeitplan gecrawlt (der durchforstungszeitplan kann nicht geändert werden). Der Crawler ruft Inhalte ab, die seit der letzten Durchforstung geändert wurden, und aktualisiert den Index. Wenn Sie sicherstellen möchten, dass Inhalt gecrawlt wird und der Index aktualisiert wird, beachten Sie Folgendes:

- Stellen Sie sicher, dass Inhalte gefunden werden können, indem [Websiteinhalte durchsuchbar gemacht](https://docs.microsoft.com/sharepoint/make-site-content-searchable)werden.

- Wenn Sie eine verwaltete Eigenschaft geändert oder die Zuordnung von durchforstete und verwalteten Eigenschaften geändert haben, muss die Website erneut durchforstet werden, bevor Ihre Änderungen im Suchindex wiedergegeben werden. 

    Da Ihre Änderungen im Suchschema und nicht auf der tatsächlichen Website vorgenommen werden, wird die Website vom Crawler nicht automatisch neu indiziert. 

    Weitere Informationen finden Sie unter [Manuelles anfordern der Durchforstung und erneuten Indizierung einer Website, einer Bibliothek oder einer Liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Warten Sie mindestens 24 Stunden nach der manuellen Anforderung einer Durchforstung und der vollständigen erneuten Indizierung, um zu sehen, ob noch ein Problem auftritt. 

    Wenn seit dem Initiieren der Durchforstung und der vollständigen erneuten Indizierung mehr als 24 Stunden vergangen sind, melden Sie sich einen Supportfall an. In vielen Fällen arbeiten wir bereits an einer Lösung. Geben Sie uns mindestens 24 Stunden, um eine Lösung zu vervollständigen.

> [!IMPORTANT]
> Wenn eine Website, ein Dokument (Bibliothek) oder eine Liste gelöscht wurde und weiterhin in den Suchergebnissen angezeigt wird, sollten Benutzer eine **Fehler 404-Datei** erhalten, die nicht gefunden wurde, wenn Sie versuchen, darauf zuzugreifen. Dieses Problem sollte bei weiteren Untersuchungen als Supportfall protokolliert werden. 



