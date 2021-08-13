---
title: identisch mit dateiname ist am besten geeignet
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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918894"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Erforderlicher Alchemy-Header H1, H2 funktioniert nicht."
Bewährte Methoden und Richtlinien für die Alchemy-Erstellung:

1. **Schachteln Sie Alchemy-Insights nicht in Ordnern**. Dadurch wird die URL-Struktur beschädigt. Wir befassen uns damit, dies zu beheben.
1. Dateien im Ordner **"AlchemyInsights"** sollten Dateinamen in Kleinbuchstaben mit Bindestrichen für Leerzeichen aufweisen. **_How-to-enable-litigation-hold_**.
    1. Schließen Sie die Regel-ID oder Bucket-ID aus dem [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) in das Feld "ms.custom" ein. Ex. ***ms.custom: 100021***
1. Verwenden Sie die restlichen Metadaten oben in dieser Datei als Vorlage.
1. Navigieren Sie im [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net)zum Abschnitt **Customer Insight Title:** und verwenden Sie diesen als Ausgangspunkt für Ihren H1-Titel für den Einblick. 
    > [!NOTE]
    > Alemy Insights DARF nur einen einzelnen H1 oben haben, sonst werden sie in der Produktion beschädigt. H2s werden nicht gerendert, verwenden Sie daher **fett** oder andere Konventionen, um separate Abschnitte zu kennzeichnen.
1. Füllen Sie als Nächstes den Textkörper mithilfe des Entwurfsmaterials im Customer Insights Abschnitt der Seite "Alchemy-Regel" aus.
    1. Aufzählungen sind in Ordnung
    1. Auch nummerierte Listen
    1. **Fett** und *kursiv* sind a-ok
    1. Links sollten immer **entweder "Links zum Web"/externen** oder **Deep-Links zu UI-Elementen** sein, nicht zu internen Links.
    1. Bilder werden derzeit nicht offiziell unterstützt, aber sie sind auf der Roadmap.

Und dies ist eigentlich schon ein wenig zu lang. Bewährte Methode ist etwa 400 Zeichen ---------------------------------

Sobald Ihre Inhalte bereit sind, ziehen Sie sie in die Live-Verzweigung. Wechseln Sie dann zum [Alchemy Partner-Portal,](https://alchemyportal.azurewebsites.net) und geben Sie den Dateinamen in das FELD "URL" ein. 