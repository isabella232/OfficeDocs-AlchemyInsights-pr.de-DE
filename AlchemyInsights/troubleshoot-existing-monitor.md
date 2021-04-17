---
title: Problembehandlung bei vorhandenen Monitoren
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824578"
---
# <a name="troubleshoot-an-existing-monitor"></a>Problembehandlung für einen vorhandenen Monitor

Probieren Sie diese Lösungen aus, um probleme mit einem Monitor zu beheben. 

**Aktualisieren sie die Anzeige Ihres Monitors:**

Drücken Sie die folgenden Tasten gleichzeitig: Windows-TASTE + STRG + Umschalt + B. Dadurch wird die Kommunikation mit dem Grafiktreiber aktualisiert. Ihre Monitore blinken kurz und kommen nach ein paar Sekunden zurück.

**Problembehandlung bei der Monitorhardware:**

1. Ziehen Sie das Kabel ab, das Ihren PC mit Ihrem Monitor verbindet, und schließen Sie es wieder an.
2. Trennen Sie alle nicht wesentlichen Geräte von Ihrem PC (z. B. Adapter oder Dockingstationen).

**Wenn Sie kürzlich ein Update auf Ihrem PC installiert haben, können Sie ein Rollback des Anzeigetreibers starten:**

1. Wählen **Sie Start** aus, geben Sie **Geräte-Manager** ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.
2. Erweitern Sie **den Abschnitt Anzeigeadapter,** klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Eigenschaften aus.**
3. Navigieren Sie zur **Registerkarte Treiber,** und wählen Sie **Roll Back Driver aus.** <br>
Hinweis: Wenn dies nicht verfügbar ist oder  ausgegraut ist, wählen Sie in den folgenden Optionen Nein aus, um zum nächsten Schritt zu wechseln.
4. Möglicherweise müssen Sie Ihren PC neu starten, bevor diese Änderungen wirksam werden.

**Deinstallieren und installieren Sie den Anzeigetreiber:**

1. Wählen **Sie Start** aus, geben Sie **Geräte-Manager** ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.
2. Erweitern Sie **den Abschnitt Anzeigeadapter,** klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Gerät deinstallieren aus.** 
3. Wählen Sie das Feld neben **Treibersoftware für dieses Gerät löschen aus,** und wählen Sie **Deinstallieren aus.**<br>
Hinweis: Sie werden möglicherweise aufgefordert, Ihren Computer zu diesem Zeitpunkt neu zu starten. Notieren Sie sich vor dem Neustart unbedingt die restlichen Anweisungen.
4. Öffnen Sie den Geräte-Manager erneut.
5. Erweitern Sie **den Abschnitt Adapter anzeigen,** klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Treiber aktualisieren aus.**
6. Wählen **Sie Automatisch nach Updatetreibersoftware suchen aus,** und befolgen Sie die Installationsanweisungen.