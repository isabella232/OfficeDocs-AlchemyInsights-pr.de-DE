---
title: Moderne Website als Stammwebsite
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753903"
---
# <a name="modern-site-as-root-site"></a>Moderne Website als Stammwebsite

Wir haben mit dem Rollout eines neuen Features begonnen, mit dem Sie [ihre klassische Websitestamm Website mit einer modernen Website austauschen](https://docs.microsoft.com/sharepoint/modern-root-site)können. Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , um den Speicherort einer Website während der Archivierung der ursprünglichen Website mit einer anderen Website zu vertauschen. Für beide Team Websites (nicht verbunden mit einer Gruppe) und Kommunikationswebsite verfügbar.

>[!Important]
> Löschen Sie Ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen. Dies wird von Microsoft nicht unterstützt. Wenn Sie die Stammwebsite löschen, können alle SharePoint-Websites in Ihrer Organisation erst für alle Benutzer zugänglich gemacht werden, wenn Sie die Website wiederherstellen oder eine neue Website mit derselben URL erstellen. Diese Funktion wird über das Nachrichtencenter kommuniziert. Sie sollten davon ausgehen, dass das Feature in Ihrem Mandanten in Kürze aktiviert wird.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austauschen von Websites
- Die Zielwebsite gibt möglicherweise einen Fehler "nicht gefunden" (HTTP 404) für eine kurze Zeit zurück.
- Der Inhalt muss erneut durchforstet werden, um den Suchindex zu aktualisieren. Es ist kein manueller Schritt erforderlich, dies erfolgt automatisch.
- Alles, was von "statischen" Links (wie Dateisynchronisierung und OneNote-Dateien) abhängig ist, muss manuell korrigiert werden.
- Project Server-Websites müssen möglicherweise überprüft werden, um sicherzustellen, dass Sie weiterhin ordnungsgemäß zugeordnet sind. 
