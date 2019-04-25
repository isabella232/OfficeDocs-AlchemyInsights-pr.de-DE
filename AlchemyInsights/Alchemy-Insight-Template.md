---
title: identisch mit filename am besten
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366330"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Erforderlicher Alchemy-Header H1, H2 funktioniert nicht.
Bewährte Methoden und Richtlinien für die Erstellung von Alchemie:

1. **Verschachteln Sie Alchemy Insights nicht in Ordnern**– dadurch wird die URL-Struktur unterbrochen. Wir untersuchen, dies zu beheben.
1. Dateien im Ordner **AlchemyInsights** sollten Kleinbuchstaben-Dateinamen mit Bindestrichen für Leerzeichen enthalten. ***How-to-enable-Litigation-Hold***.
    1. Schließen Sie die Regel-ID oder die Bucket-ID aus dem [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) in das Feld ms. Custom ein. Ex. ***ms. Custom: 100021***
1. Verwenden Sie die restlichen Metadaten am Anfang dieser Datei als Vorlage.
1. Navigieren Sie im [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)zum Abschnitt **Customer Insight Title:** und verwenden Sie diesen als Ausgangspunkt für Ihren H1-Titel für die Einblicke. 
    > [!NOTE]
    > Alchemy inSights muss oben nur einen einzelnen H1 haben, oder Sie werden in der Produktion unterbrochen. H2s nicht rendern, verwenden Sie daher **Fett** oder andere Konventionen, um separate Abschnitte anzuzeigen.
1. Als nächstes füllen Sie den Textkörper mit dem Entwurfsmaterial im Abschnitt Kunden einBlicke auf der Seite Alchemy Rule aus.
    1. AufZählungslisten sind in Ordnung
    1. Nummerierte Listen
    1. **Fett** und *kursiv* sind a-OK
    1. Links sollten immer entweder **"Links zu Web"/External** oder **Deep-Links zu UI-Elementen**, nicht interne Links.
    1. Bilder werden zu diesem Zeitpunkt nicht offiziell unterstützt, aber es steht in der Roadmap.

Und das ist wirklich schon ein bisschen zu lang. Die bewährte Methode umfasst ungefähr 400 Zeichen---------------------------------

Sobald Ihr Inhalt fertig ist, ziehen Sie ihn in die Live-Verzweigung. Wechseln Sie dann zum [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das Feld URL ein. M