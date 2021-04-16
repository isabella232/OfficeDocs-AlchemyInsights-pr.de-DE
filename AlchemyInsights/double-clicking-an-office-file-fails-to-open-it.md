---
title: Doppelklicken auf eine Office-Datei kann nicht geöffnet werden
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814804"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Doppelklicken auf eine Office-Datei kann nicht geöffnet werden

Nach dem Doppelklicken auf eine Office-Datei wird möglicherweise das Programm geöffnet, aber die Datei selbst wird nicht geöffnet. Oder Sie erhalten den Fehler: "Beim Senden des Befehls an das Programm ist ein Problem aufgetreten." Dafür gibt es viele Ursachen, aber die beiden gängigsten Lösungen sind:

- Stellen Sie in Excel sicher, dass die Option DDE deaktiviert ist. Die Option kann gefunden werden, indem Sie eine neue Arbeitsmappe erstellen und dann **Datei > Optionen > auswählen.** Deaktivieren Sie **im Abschnitt Allgemein** die Option Andere Anwendungen ignorieren, die dynamic Data Exchange **(DDE) verwenden.**

- Führen Sie eine Onlinereparatur aus, um die Standardeinstellungen wiederherzustellen. Klicken Sie auf die Schaltfläche Windows Start, und suchen Sie nach "Systemsteuerung". Öffnen Sie **die Systemsteuerung,** und wechseln Sie zu **Programme > Programme und Features**. Klicken Sie dann mit der **rechten maustaste Microsoft Office [Version]** und wählen **Sie Ändern > Onlinereparatur aus.**

Wenn keine dieser Lösungen funktioniert, finden Sie im Supportartikel eine vollständigere Lösungsliste, wenn sie beim Doppelklicken auf eine [Office-Datei nicht geöffnet werden kann.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
