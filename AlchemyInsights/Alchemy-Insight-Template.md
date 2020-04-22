---
title: identisch mit filename ist am besten
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676532"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Erforderlicher Alchemy-Header H1, H2 funktioniert nicht.
Bewährte Methoden und Richtlinien für die Erstellung von Alchemy-Autoren:

1. **Alchemy Insights in Folders nicht Schachteln**-dadurch wird die URL-Struktur unterbrochen. Wir untersuchen, wie Sie dieses Problem beheben.
1. Dateien im Ordner **AlchemyInsights** sollten klein geschriebene Dateinamen mit Bindestrichen für Leerzeichen (ex) enthalten. ***How-to-enable-Litigation-Hold***.
    1. Schließen Sie die Regel-ID oder Bucket-ID aus dem [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) in das Feld ms. Custom ein. Ex. ***ms. Custom: 100021***
1. Verwenden Sie die restlichen Metadaten oben in dieser Datei als Vorlage.
1. Navigieren Sie im [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)nach unten zum Abschnitt **Kunden Einblicke Title:** , und verwenden Sie diesen als Ausgangspunkt für den H1-Titel für die Einblicke. 
    > [!NOTE]
    > Alchemy Insights muss nur ein einzelnes H1 am oberen Rand aufweisen, oder die Produktion wird unterbrochen. H2s Rendern weder so verwenden Sie **Fett** oder andere Konventionen, um separate Abschnitte zu bedeuten.
1. Geben Sie als nächstes den Textkörper mithilfe des Entwurfs Materials im Abschnitt Kunden Einblicke der Seite Alchemy Rule ein.
    1. Aufzählungslisten sind in Ordnung
    1. Nummerierte Listen
    1. **Fett** und *kursiv* sind a-OK
    1. Links sollten immer entweder **"Links to Internet"/External** oder **Deep-Links zu Benutzeroberflächenelementen**sein, keine internen Links.
    1. Bilder werden zu diesem Zeitpunkt nicht offiziell unterstützt, aber Sie sind in der Roadmap.

Und das ist wirklich schon ein bisschen zu lang. Bewährte Methode sind etwa 400 Zeichen---------------------------------

Nachdem der Inhalt abgeschlossen ist, ziehen Sie ihn in den Live-Zweig. Wechseln Sie dann zum [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das URL-Feld ein. 