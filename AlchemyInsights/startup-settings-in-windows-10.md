---
title: Starteinstellungen in Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828151"
---
# <a name="startup-settings-in-windows-10"></a>Starteinstellungen in Windows 10

**Ändern, welche Apps beim Start automatisch ausgeführt werden**

1. Wechseln Sie [zu Einstellungen > Apps > Start](ms-settings:startupapps?activationSource=GetHelp).

2. Stellen Sie sicher, dass alle Apps, die Sie beim Start ausführen möchten, aktiviert **ist.**

**Hinzufügen einer App, die beim Start automatisch ausgeführt werden soll**

1. Klicken oder tippen Sie **auf Starten,** und suchen Sie die App, die Sie beim Start ausführen möchten.

2. Klicken Sie mit der rechten Maustaste auf die App, klicken Sie auf **Weitere**, und klicken Sie dann **auf Dateispeicherort öffnen.** Dadurch wird der Speicherort geöffnet, an dem die Verknüpfung zur App gespeichert wird. Wenn keine Option für dateispeicherort öffnen verfügbar ist, bedeutet dies, dass die App beim Start nicht ausgeführt werden kann.

3. Wenn der Dateispeicherort geöffnet ist, drücken Sie die **Windows-Logotaste + R**, geben Sie **shell:startup** ein, und klicken Sie dann auf **OK**. Dadurch wird der Startordner geöffnet.

4. Kopieren Sie die Verknüpfung aus dem Dateispeicherort in den Startordner, und fügen Sie sie in die App ein.

**Erweiterte Startoptionen (einschließlich abgesicherter Modus, UEFI-Einstellungen und Starten von einem anderen Gerät)**

1. Speichern Sie Ihre Arbeit, und schließen Sie alle geöffneten Dokumente, da mit diesen Schritten Ihr PC neu gestartet wird.

2. Wechseln Sie [zu Einstellungen > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Klicken **Sie unter Erweiterter** Start jetzt **auf Neu starten.** 

4. Nach dem Neustart des PCs auf dem Bildschirm Option auswählen:

    - Klicken Sie auf Verwenden eines Geräts, um von einem Gerät wie einem USB-Laufwerk **zu starten.**

    - Klicken Sie zum Eingeben der UEFI-Einstellungen (manchmal als BIOS-Setup bezeichnet) auf Problembehandlung > Erweiterte Optionen **> UEFI-Firmwareeinstellungen**. 

    - Um in den abgesicherten Modus zu wechseln oder erweiterte Starteinstellungen zu ändern, klicken Sie auf Problembehandlung > Erweiterte Optionen > **Starteinstellungen,** und klicken Sie dann auf **Neu starten**. Möglicherweise werden Sie aufgefordert, Ihren [BitLocker-Wiederherstellungsschlüssel ein eingeben.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Klicken Sie nach dem neustarten des PCs auf die Starteinstellung, die Sie verwenden möchten.