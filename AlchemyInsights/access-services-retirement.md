---
title: Ruhestand "Access Services"
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359344"
---
# <a name="access-services-retirement"></a>Ruhestand "Access Services"

Wie wir ursprünglich in MC97576 angekündigt haben, im März 2017 und im vergangenen Jahr weiter kommuniziert haben, werden Access Services von Office 365 zurückgezogen. Die nächste Phase in diesem Prozess wird das Entfernen von Access-Webdatenbanken sein, die SharePoint-Listen als zugrunde liegender Datenspeicher verwenden.

**Wie wirkt sich dies auf mich aus?**

Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden apps bis April 2020 Herunterfahren.

**Was muss ich tun, um diese Änderung vorzubereiten?**

Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen. Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der Access-apps zu erhalten, die von Websites verwendet werden.

Es gibt verschiedene Möglichkeiten zum Migrieren von Access-Daten Bank Datenbanken:

- Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.
- Außerdem wird empfohlen, Microsoft PowerApps als Alternative Plattform zum Erstellen von codelosen Geschäftslösungen für das Internet und mobile Geräte zu erforschen.