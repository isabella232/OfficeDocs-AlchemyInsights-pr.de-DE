---
title: Behandeln von Audioproblemen in Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833290"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Problembehandlung bei Audioproblemen in Windows 10

**Ausführen der Audioproblemesbehandlung**

1.  Öffnen Sie [die Problembehandlungseinstellungen](ms-settings:troubleshoot).

2.  Wählen **Sie Wiedergeben von Audio** Ausführen der  >  **Problembehandlung aus.**

**Festlegen des Standardgeräts**

Wenn Sie eine Verbindung mit einem Audiogerät über USB oder HDMI herstellen, müssen Sie dieses Gerät möglicherweise als Standard festlegen:

1. Öffnen **Sie**  >  **Startsound,** und wählen Sie dann **sound** or Change **system sounds** aus der Liste der Ergebnisse aus.

2.  Wählen Sie **auf der** Registerkarte Wiedergabe ein Gerät aus, wählen Sie **Standard festlegen** und dann **OK aus.**

**Überprüfen von Kabeln, Lautstärke, Lautsprechern und Kopfhörern**

1. Überprüfen Sie die Lautsprecher- und Kopfhörerverbindungen auf lose Kabel, und stellen Sie sicher, dass sie mit der richtigen Buchse verbunden sind.

2. Überprüfen Sie Ihre Energie- und Lautstärkestufen, und versuchen Sie, alle Volumesteuerelemente hoch zu schalten.

3. Einige Lautsprecher und Apps verfügen über eigene Lautstärkesteuerelemente. Sie müssen sie möglicherweise alle überprüfen, um sicherzustellen, dass sie auf den richtigen Ebenen sind.

4. Versuchen Sie, eine Verbindung über einen anderen USB-Port zu herstellen.

**Hinweis:** Denken Sie daran, dass Ihre Lautsprecher möglicherweise nicht funktionieren, wenn Kopfhörer angeschlossen sind.

**Überprüfen des Geräte-Managers**

So stellen Sie sicher, dass die Treiber auf dem neuesten Stand sind:

1. Wählen **Sie Start** aus, geben Sie Device **Manager** ein, und wählen Sie dann **Geräte-Manager** in der Liste der Ergebnisse aus.

2. Wählen **Sie unter Sound-, Video-** und Gamecontroller Ihre  Soundkarte aus, öffnen Sie sie, wählen Sie die Registerkarte Treiber aus, und wählen Sie **Updatetreiber aus.**

**Hinweis:** Wenn Windows keinen neuen Treiber findet, suchen Sie auf der Website des Geräteherstellers nach einem Treiber, und befolgen Sie die Anweisungen.

**Erneutes Installieren des Treibers**

Wenn Sie nicht über den Geräte-Manager aktualisieren oder einen neuen Treiber auf der Website des Herstellers finden können, führen Sie die folgenden Schritte aus:

1. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf den Audiotreiber (oder halten Sie ihn), und wählen Sie **Deinstallieren aus.** Starten Sie Ihr Gerät neu, und Windows versucht, den Treiber neu zu installieren.

2. Wenn die Neuinstallation des Treibers nicht funktioniert, versuchen Sie, den generischen Audiotreiber zu verwenden, der mit Windows ausgestattet ist. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf Ihren **Audiotreiber**> Treibersoftware aktualisieren Durchsuchen Sie meinen Computer nach Treibersoftware Lassen Sie mich aus einer Liste der Gerätetreiber auf meinem Computer auswählen, wählen Sie High  >    >  Definition **Audio Device** aus, wählen Sie **Weiter** aus, und folgen Sie den Anweisungen zur Installation.
