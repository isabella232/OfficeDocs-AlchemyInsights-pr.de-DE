---
title: Beheben von Bluetooth-Problemen in Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730158"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Beheben von Bluetooth-Problemen in Windows 10

Wenn das Bluetooth-Symbol fehlt oder Bluetooth nicht aktiviert oder deaktiviert werden kann, möchten Sie möglicherweise die Bluetooth-Problembehandlung ausführen. [Öffnen Sie die Problembehandlungseinstellungen](ms-settings:troubleshoot), klicken Sie unter **Suchen und beheben anderer Probleme**auf **Bluetooth** , und klicken Sie dann auf **Problembehandlung ausführen**.

Wenn das Bluetooth-Symbol nicht angezeigt wird, aber Bluetooth im Geräte-Manager angezeigt wird:

1. Klicken Sie im Geräte-Manager auf **Bluetooth**. Halten Sie den Bluetooth-Adapternamen gedrückt (oder klicken Sie mit der rechten Maustaste), und klicken Sie auf **Gerät deinstallieren**.

2. Fahren Sie Ihr Windows-Gerät herunter, warten Sie einige Sekunden, und schalten Sie es dann wieder ein. Der Treiber wird von Windows erneut installiert.

Wenn Sie vor kurzem Windows 10-Updates installiert oder auf Windows 10 aktualisiert haben, sollten Sie nach Treiberupdates suchen:

1. Klicken Sie im Geräte-Manager auf **Bluetooth**, und klicken Sie dann auf den Namen des Bluetooth-Adapters (der das Wort "Radio" enthalten kann).

2. Halten Sie den Bluetooth-Adapter gedrückt (oder klicken Sie mit der rechten Maustaste darauf), und klicken Sie dann auf automatische **Treiber**  >  **Suche aktualisieren für aktualisierte Treibersoftware**. Führen Sie die Schritte aus, und klicken Sie dann auf **Schließen**.

      - Wenn Windows keinen neuen Bluetooth-Treiber finden kann, besuchen Sie die Website des PC-Herstellers, und laden Sie von dort den neuesten Bluetooth-Treiber herunter.

    - Nachdem Sie das Programm heruntergeladen haben, klicken Sie auf **Treiber aktualisieren**  >  **Durchsuchen**nach  >  dem Speicherort der Treiberdateien**Durchsuchen** des Speicherorts, an dem die Treiberdateien gespeichert sind > **OK**  >  **Next**, und führen Sie die folgenden Schritte aus, um zu installieren.

3. Nachdem Sie den aktualisierten Treiber installiert haben, starten Sie den Computer neu, und überprüfen Sie dann, ob das Verbindungsproblem behoben wurde.

Weitere Informationen zur Behandlung von Bluetooth-Problemen finden Sie im vollständigen Artikel Beheben von [Bluetooth-Problemen in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
