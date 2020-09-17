---
title: Verwenden von Fingerabdruck-Unlock-Option in Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795243"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Verwenden von Fingerabdruck-Unlock-Option in Windows 10

**Windows Hello-Fingerabdruck aktivieren**

Wenn Sie Windows 10 mit Ihrem Fingerabdruck entsperren möchten, müssen Sie Windows Hello Fingerprint einrichten, indem Sie mindestens einen Finger hinzufügen (sodass Windows erkennen kann, dass er Sie erkennt). 

1. Wechseln Sie zu **Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Die verfügbaren Anmeldeoptionen werden aufgelistet. Zum Beispiel:

    ![Anmeldeoptionen.](media/sign-in-options.png)

2. Klicken oder tippen Sie auf **Windows Hello Fingerprint**, und klicken Sie dann auf **Einrichten**. Klicken Sie im Fenster Hello Setup von Windows auf **Erste Schritte**. Der Fingerabdrucksensor wird aktiviert, und Sie werden aufgefordert, Ihren Finger auf den Sensor zu setzen:

   ![Fingerabdrucksensor.](media/fingerprint-sensor.png)

3. Befolgen Sie die Anweisungen, die Sie bitten, Ihren Finger wiederholt zu überprüfen. Wenn dieser Vorgang abgeschlossen ist, haben Sie die Möglichkeit, weitere Finger hinzuzufügen, die Sie möglicherweise für die Anmeldung verwenden möchten. Wenn Sie sich das nächste Mal bei Windows 10 anmelden, haben Sie die Möglichkeit, Ihren Fingerabdruck zu verwenden.

**Windows Hello Fingerabdruck nicht als Anmeldeoption verfügbar**

Wenn Windows Hello Fingerabdruck nicht als Option in den **Anmeldeoptionen**angezeigt wird, bedeutet dies, dass Windows keine Fingerabdruckleser/Scanner kennt, die an Ihren PC angeschlossen sind, oder dass eine Systemrichtlinie deren Verwendung verhindert (beispielsweise wenn Ihr PC von Ihrem Arbeitsplatz verwaltet wird). Zur Problembehandlung: 

1. Wählen Sie die Schaltfläche **Start** in der Taskleiste aus, und suchen Sie nach **Geräte-Manager**.

2. Klicken oder tippen Sie auf, um den **Geräte-Manager**zu öffnen.

3. Erweitern Sie im Geräte-Manager biometrische Geräte, indem Sie auf dessen Chevron klicken.

   ![Biometrische Geräte.](media/biometric-devices.png)

4. Ihr Fingerabdruck-Scanner sollte als biometrisches Gerät wie der Synaptics WBDI-Scanner aufgeführt werden:

   ![Biometrische Geräte.](media/biometric-devices-expanded.png)

5. Wenn Ihr Fingerabdruckscanner nicht angezeigt wird und der Scanner in Ihren PC integriert ist, wechseln Sie zur Website des PC-Herstellers. Suchen Sie im Abschnitt technischer Support für Ihr PC-Modell nach einem Windows 10-Treiber für einen Scanner, den Sie installieren können.

6. Wenn der Scanner vom PC getrennt ist (über USB angeschlossen), wechseln Sie zur Website des Scanner-Herstellers, um die Gerätetreibersoftware von Windows 10 für das Scanner-Modell zu finden und zu installieren.
