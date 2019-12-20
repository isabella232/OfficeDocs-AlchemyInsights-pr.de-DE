---
title: Beheben von Problemen mit Audiodaten in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796123"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Problembehandlung bei Audioproblemen in Windows 10

**Ausführen der Audioproblem-Problembehandlung**

Die Audioproblembehandlung kann die Audioprobleme möglicherweise automatisch beheben: 

1. Wählen Sie **Start**, geben Sie **Problembehandlung**ein, und wählen Sie dann in der Ergebnisliste die Option **Problembehandlung** aus. 
2. Wählen Sie **Wiedergabe von Audio** > **Ausführen der Problembehandlung**aus.

**Überprüfen von Kabeln, Lautstärke, Lautsprechern und Kopfhörern**

- Überprüfen Sie die Lautsprecher-und Kopfhöreranschlüsse auf lose Kabel, und stellen Sie sicher, dass Sie mit der richtigen Buchse verbunden sind.
- Überprüfen Sie die Leistungs-und Lautstärkewerte, und drehen Sie alle Lautstärkeregler nach oben.
- Einige Lautsprecher und apps verfügen über eigene Volumen Steuerelemente und müssen möglicherweise alle überprüfen, um sicherzustellen, dass Sie auf der richtigen Ebene sind.
- Versuchen Sie, eine Verbindung über einen anderen USB-Port herzustellen.
- **Hinweis:** Denken Sie daran, dass Ihre Lautsprecher möglicherweise nicht funktionieren, wenn Kopfhörer angeschlossen sind.

**Überprüfen des Geräte-Managers**

So stellen Sie sicher, dass die Treiber auf dem neuesten Stand sind:

- Wählen Sie **Start**aus, geben Sie **Geräte-Manager**ein, und wählen Sie dann in der Ergebnisliste den **Geräte-Manager** aus.

2. Wählen Sie unter **Sound-, Video-und Gamecontroller**Ihre Soundkarte aus, öffnen Sie Sie, wählen Sie die Registerkarte **Treiber** aus, und wählen Sie **Treiber aktualisieren**aus. 

**Hinweis:** Wenn Windows keinen neuen Treiber findet, suchen Sie auf der Website des Geräteherstellers nach einem und folgen Sie den Anweisungen.

**Installieren des Treibers**

Wenn Sie nicht über den Geräte-Manager aktualisieren oder einen neuen Treiber auf der Website des Herstellers finden können, führen Sie die folgenden Schritte aus: 

1. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf den Audiotreiber (oder halten Sie ihn gedrückt), und wählen Sie **deinstallieren**aus. Starten Sie Ihr Gerät neu, und Windows versucht, den Treiber erneut zu installieren.

2. Wenn die Neuinstallation des Treibers nicht funktioniert, versuchen Sie, den generischen Audiotreiber zu verwenden, der mit Windows ausgeliefert wird. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf den Audiotreiber #a0 **Update Driver Software** > auf**meinem Computer nach Treibersoftware** > suchen**lassen Sie mich aus einer Liste der Gerätetreiber auf meinem Computer**auswählen, wählen Sie **High Definition Audio Device**aus, wählen Sie **weiter**aus, und befolgen Sie die Anweisungen, um es zu installieren.

**Festlegen des Standardgeräts**

Wenn Sie über USB oder HDMI eine Verbindung mit einem Audiogerät herstellen, müssen Sie dieses Gerät möglicherweise als Standard festlegen: 

1. Wählen Sie **Start**, geben Sie **Sound**ein, und wählen Sie dann **Sound** aus der Ergebnisliste aus, oder **Ändern Sie Systemsounds** .

2. Wählen Sie auf der Registerkarte **Wiedergabe** ein Gerät aus, wählen Sie **Standard festlegen**aus, und wählen Sie dann **OK**aus.

