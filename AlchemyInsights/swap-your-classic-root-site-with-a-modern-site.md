---
title: Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501078"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.

Wenn Ihre Umgebung vor dem 2019 April eingerichtet wurde, können Sie die Stammwebsite mithilfe von Microsoft PowerShell in eine moderne Website ändern:

- Wenn Sie eine andere Website als Stammwebsite verwenden möchten, können Sie die Stammwebsite durch diese ersetzen (tauschen). 
    - Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , um den Speicherort einer Website während der Archivierung der ursprünglichen Website mit einer anderen Website zu vertauschen. Für beide Team Websites (nicht verbunden mit einer Gruppe) und Kommunikationswebsite verfügbar. 

- In Kürze werden zusätzliche Funktionen eingeführt, mit denen Sie die Inhalte auf der Website weiterhin verwenden, die vorhandene Website jedoch in eine Kommunikationswebsite umwandeln können. 
>[!Important]
>Diese Funktionen werden schrittweise ausgeführt. Fahren Sie mit dem Überprüfen des Office 365 Nachrichten Centers auf Updates fort. 

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austauschen von Websites

- Die Zielwebsite gibt möglicherweise einen Fehler "nicht gefunden" (HTTP 404) für eine kurze Zeit zurück.
- Der Inhalt muss erneut durchforstet werden, um den Suchindex zu aktualisieren. Es ist kein manueller Schritt erforderlich – Dies erfolgt automatisch.
- Alles, was von "statischen" Links (wie Dateisynchronisierung und OneNote-Dateien) abhängig ist, muss manuell korrigiert werden.
- Wenn es sich bei der Quellwebsite um eine organisatorische Nachrichtenwebsite handelt, aktualisieren Sie die URL.Hier erhalten Sie eine Liste aller Nachrichtenwebsites für die Organisation.
- Project Server-Websites müssen möglicherweise überprüft werden, um sicherzustellen, dass Sie weiterhin ordnungsgemäß zugeordnet sind.





