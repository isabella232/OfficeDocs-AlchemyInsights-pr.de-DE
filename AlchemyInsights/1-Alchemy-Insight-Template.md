---
title: 'identisch mit filename ist am besten [RULE #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634503"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Erforderlicher Alchemy-Header H1, H2 funktioniert nicht.
Bewährte Methoden und Richtlinien für die Erstellung von Alchemie:

1. **Verschachteln Sie Alchemy Insights nicht in Ordnern**– dadurch wird die URL-Struktur unterbrochen. Wir untersuchen, dies zu beheben.
1. Dateien im Ordner **AlchemyInsights** sollten über das [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) im Dateinamen Regel-ID und Regelname enthalten.
    1. Ex. ***976-enable-Litigation-Hold***
1. Verwenden Sie die Metadaten am Anfang dieser Datei als Vorlage. Es ist nichts anderes erforderlich.
1. Navigieren Sie im [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)zum Abschnitt **Customer Insight Title:** und verwenden Sie diesen als Ausgangspunkt für Ihren H1-Titel für die Einblicke. 
    > [!NOTE]
    > Alchemy inSights muss oben nur einen einzelnen H1 haben, oder Sie werden in der Produktion unterbrochen. H2s nicht rendern, verwenden Sie daher **Fett** oder andere Konventionen, um separate Abschnitte anzuzeigen.
1. Als nächstes füllen Sie den Textkörper mit dem Entwurfsmaterial im Abschnitt Kunden einBlicke auf der Seite Alchemy Rule aus.
    1. AufZählungslisten sind in Ordnung
    1. Nummerierte Listen
    1. **Fett** und *kursiv* sind a-OK
    1. Links sollten immer entweder **"Links zu Web"/External** oder **Deep-Links zu UI-Elementen**, nicht interne Links.

Und das ist wirklich schon ein bisschen zu lang. Die bewährte Methode umfasst ungefähr 400 Zeichen---------------------------------

Sobald Ihr Inhalt fertig ist, ziehen Sie ihn in die Live-Verzweigung. Wechseln Sie dann zum [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das Feld URL ein. Vergewissern Sie sich, dass einBlicke überprüft und veröffentlicht werden, und klicken Sie auf Regel aktualisieren. **(Dies wird in der neuen Version des Portals schöner aussehen-Veröffentlichung in Kürze.)** 
 ![](media/for-content-team.PNG)

