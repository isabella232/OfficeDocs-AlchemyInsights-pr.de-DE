---
title: Problembehandlung für vorhandenen Monitor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690710"
---
# <a name="troubleshoot-an-existing-monitor"></a>Problembehandlung bei einem vorhandenen Monitor

Versuchen Sie diese Lösungen zur Problembehandlung für einen Monitor. 

**Aktualisieren Sie die Anzeige Ihres Monitors:**

Drücken Sie gleichzeitig die folgenden Tasten: Windows-Taste + STRG + UMSCHALT + B. Dadurch wird die Kommunikation mit Ihrem Grafiktreiber aktualisiert. Ihre Monitore blinken kurz und kommen nach ein paar Sekunden zurück.

**Problembehandlung bei der Hardwareüberwachung:**

1. Ziehen Sie das Kabel, das Ihren PC mit dem Monitor verbindet, aus, und stecken Sie es wieder ein.
2. Trennen Sie alle nicht wesentlichen Geräte von Ihrem PC (wie Adapter oder Docks).

**Wenn Sie vor kurzem ein Update auf Ihrem PC installiert haben, können Sie den Bildschirmtreiber wiederherstellen:**

1. Wählen Sie **Start**, geben Sie **Geräte-Manager**ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.
2. Erweitern Sie den Abschnitt **Anzeigeadapter** , klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Eigenschaften**aus.
3. Navigieren Sie zur Registerkarte **Treiber** , und wählen Sie **Rollback Driver**aus. <br>
Hinweis: Wenn diese Option nicht verfügbar ist oder abgeblendet ist, wählen Sie in den Optionen unten die Option **Nein** aus, um zum nächsten Schritt zu gelangen.
4. Möglicherweise müssen Sie Ihren PC neu starten, bevor diese Änderungen wirksam werden.

**Deinstallieren Sie den Anzeigetreiber, und installieren Sie ihn neu:**

1. Wählen Sie **Start**, geben Sie **Geräte-Manager**ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.
2. Erweitern Sie den Abschnitt **Anzeigeadapter** , klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Gerät deinstallieren**aus. 
3. Aktivieren Sie das Kontrollkästchen neben **die Treibersoftware für dieses Gerät löschen** , und wählen Sie **deinstallieren**aus.<br>
Hinweis: Sie werden möglicherweise aufgefordert, Ihren Computer zu diesem Zeitpunkt neu zu starten. Achten Sie darauf, dass Sie die restlichen Anweisungen vor dem Neustart notieren.
4. Öffnen Sie erneut den Geräte-Manager.
5. Erweitern Sie den Abschnitt **Anzeigeadapter** , klicken Sie mit der rechten Maustaste auf Ihren Anzeigeadapter, und wählen Sie **Treiber aktualisieren**aus.
6. Wählen Sie **Automatische Suche für Update Treibersoftware** aus, und befolgen Sie die Installationsanweisungen.