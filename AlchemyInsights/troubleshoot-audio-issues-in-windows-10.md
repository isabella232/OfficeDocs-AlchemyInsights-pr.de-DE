---
title: Beheben von Problemen mit Audiodaten in Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750306"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Problembehandlung bei Audioproblemen in Windows 10

**Ausführen der Audioproblem-Problembehandlung**

1.  Öffnen Sie die [Problembehandlungseinstellungen](ms-settings:troubleshoot).

2.  Wählen Sie **Wiedergabe von Audio**  >  **Ausführen der Problembehandlung**aus.

**Festlegen des Standardgeräts**

Wenn Sie über USB oder HDMI eine Verbindung mit einem Audiogerät herstellen, müssen Sie dieses Gerät möglicherweise als Standard festlegen:

1. Öffnen Sie **Start**  >  **Sound**, und wählen Sie dann **Sound** aus der Ergebnisliste aus, oder ändern Sie die **Systemsounds** .

2.  Wählen Sie auf der Registerkarte **Wiedergabe** ein Gerät aus, wählen Sie **Standard festlegen**aus, und wählen Sie dann **OK**aus.

**Überprüfen von Kabeln, Lautstärke, Lautsprechern und Kopfhörern**

1. Überprüfen Sie die Lautsprecher-und Kopfhöreranschlüsse auf lose Kabel, und stellen Sie sicher, dass Sie mit der richtigen Buchse verbunden sind.

2. Überprüfen Sie die Leistungs-und Lautstärkewerte, und drehen Sie alle Lautstärkeregler nach oben.

3. Einige Lautsprecher und apps verfügen über eigene Lautstärkeregler; Möglicherweise müssen Sie alle überprüfen, um sicherzustellen, dass Sie auf der richtigen Ebene sind.

4. Versuchen Sie, eine Verbindung über einen anderen USB-Port herzustellen.

**Hinweis**: Denken Sie daran, dass Ihre Lautsprecher möglicherweise nicht funktionieren, wenn Kopfhörer angeschlossen sind.

**Überprüfen des Geräte-Managers**

So stellen Sie sicher, dass die Treiber auf dem neuesten Stand sind:

1. Wählen Sie **Start**aus, geben Sie **Geräte-Manager**ein, und wählen Sie dann in der Ergebnisliste den **Geräte-Manager** aus.

2. Wählen Sie unter **Sound-, Video-und Gamecontroller**Ihre Soundkarte aus, öffnen Sie Sie, wählen Sie die Registerkarte **Treiber** aus, und wählen Sie **Treiber aktualisieren**aus.

**Hinweis**: Wenn Windows keinen neuen Treiber findet, suchen Sie auf der Website des Geräteherstellers nach einem und folgen Sie den Anweisungen.

**Installieren des Treibers**

Wenn Sie nicht über den Geräte-Manager aktualisieren oder einen neuen Treiber auf der Website des Herstellers finden können, führen Sie die folgenden Schritte aus:

1. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf den Audiotreiber (oder halten Sie ihn gedrückt), und wählen Sie **deinstallieren**aus. Starten Sie Ihr Gerät neu, und Windows versucht, den Treiber erneut zu installieren.

2. Wenn die Neuinstallation des Treibers nicht funktioniert, versuchen Sie, den generischen Audiotreiber zu verwenden, der mit Windows ausgeliefert wird. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf den Audiotreiber > **Update Driver Software**  >  auf**meinem Computer nach Treibersoftware suchen**  >  **lassen Sie mich aus einer Liste der Gerätetreiber auf meinem Computer**auswählen, wählen Sie **High Definition Audio Device**aus, wählen Sie **weiter**aus, und befolgen Sie die Anweisungen, um es zu installieren.
