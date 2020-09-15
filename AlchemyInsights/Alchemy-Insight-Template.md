---
title: identisch mit filename ist am besten
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664133"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Erforderlicher Alchemy-Header H1, H2 funktioniert nicht."
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