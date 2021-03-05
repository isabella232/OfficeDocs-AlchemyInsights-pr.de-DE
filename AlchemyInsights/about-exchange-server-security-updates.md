---
title: Informationen Exchange Server Sicherheitsupdates
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449099"
---
# <a name="about-exchange-server-security-updates"></a>Informationen Exchange Server Sicherheitsupdates

Microsoft hat eine Reihe wichtiger Sicherheitsupdates für Exchange Server veröffentlicht. Bei den betroffenen Serverversionen handelt es sich um Updatestufen von Exchange Server 2010, 2013, 2016 und 2019. Exchange Online ist NICHT betroffen, aber wenn Sie aufgrund der Hybridkonfiguration über einige lokale Exchange-Server verfügen, sind sie potenziell anfällig.

Zum Aktualisieren Ihrer lokalen Server müssen mindestens die folgenden Versionen von Exchange ausgeführt werden:

- Exchange 2010 Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 KU 19 oder CU 18
- Exchange Server 2019 KU 8 oder CU 7

Informationen zum Speicherort von Korrekturen finden Sie in der folgenden Ankündigung: [Veröffentlicht: März 2021 Exchange Server Sicherheitsupdates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**Wichtige Hinweise:**

Die Installation von Updates funktioniert nicht, wenn auf ihren lokalen Servern keine erforderlichen Exchange-Versionen ausgeführt werden, wie in der obigen Liste angegeben.

Wenn Sie Updates manuell installieren, lesen Sie den Abschnitt "Bekannte Probleme" der Update-KB-Artikel, um wichtige Informationen zu erhalten. Sicherheitsupdates MÜSSEN über eine CMD/PowerShell-Eingabeaufforderung mit erhöhten Rechten ausgeführt werden!
