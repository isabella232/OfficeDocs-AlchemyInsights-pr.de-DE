---
title: Access Services-Ruhestand
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973918"
---
# <a name="access-services-retirement"></a>Access Services-Ruhestand

Wie wir ursprünglich in MC97576 angekündigt haben, im März 2017 und weiterhin über das vergangene Jahr kommunizieren, werden Access Services aus Office 365 zurückgezogen. Die nächste Phase dieses Prozesses ist das Entfernen von Access-Webdatenbanken, die SharePoint-Listen als zugrunde liegender Datenspeicher verwenden.

## <a name="how-does-this-affect-me"></a>Wie wirkt sich das auf mich aus?

Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden apps bis April 2020 Herunterfahren.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>Was muss ich tun, um diese Änderung vorzubereiten?

Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen. Administratoren können den [SharePoint Access-App-Scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) verwenden, um eine Bestandsaufnahme der Access-apps abzurufen, die von Websites verwendet werden. 

Es gibt mehrere Möglichkeiten zum Migrieren von Daten in Access-Webdatenbanken:

- Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.
- Außerdem wird empfohlen, Microsoft PowerApps als Alternative Plattform für die Erstellung von Unternehmenslösungen ohne Code für Web-und mobile Geräte zu erkunden.