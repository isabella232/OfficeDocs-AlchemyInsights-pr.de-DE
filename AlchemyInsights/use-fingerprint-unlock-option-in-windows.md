---
title: Verwenden der Option zum Entsperren von Fingerabdrücken in Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796676"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Verwenden der Option zum Entsperren von Fingerabdrücken in Windows 10

**Aktivieren von Windows Hello Fingerprint**

Um Windows 10 mithilfe Ihres Fingerabdrucks zu entsperren, müssen Sie Windows Hello Fingerprint einrichten, indem Sie mindestens einen Finger hinzufügen (damit Windows erkennen kann). 

1. Wechseln Sie **zu Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Verfügbare Anmeldeoptionen werden aufgelistet. Zum Beispiel:

    ![Anmeldeoptionen.](media/sign-in-options.png)

2. Klicken oder tippen **Sie auf Windows Hello Fingerprint,** und klicken Sie dann auf **Einrichten**. Klicken Sie im Windows Hello-Setupfenster auf **Erste Schritte.** Der Fingerabdrucksensor wird aktiviert, und Sie werden aufgefordert, den Finger auf dem Sensor zu platzieren:

   ![Fingerabdrucksensor.](media/fingerprint-sensor.png)

3. Befolgen Sie die Anweisungen, die Sie bitten, ihren Finger wiederholt zu scannen. Wenn dies abgeschlossen ist, können Sie andere Finger hinzufügen, die Sie möglicherweise für die Anmeldung verwenden möchten. Wenn Sie sich das nächste Mal bei Windows 10 anmelden, haben Sie die Möglichkeit, dazu Ihren Fingerabdruck zu verwenden.

**Windows Hello Fingerprint nicht als Anmeldeoption verfügbar**

Wenn Windows Hello Fingerprint nicht als Option **in** Anmeldeoptionen angezeigt wird, bedeutet dies, dass Windows keine Fingerabdruckleser/Scanner kennt, die an Ihren PC angefügt sind, oder dass eine Systemrichtlinie die Verwendung verhindert (wenn ihr PC beispielsweise von Ihrem Arbeitsplatz verwaltet wird). So behandeln Sie: 

1. Wählen Sie die **Schaltfläche Start** in der Taskleiste aus, und suchen Sie nach **Device Manager**.

2. Klicken oder tippen Sie, um den **Geräte-Manager zu öffnen.**

3. Erweitern Sie im Geräte-Manager biometrische Geräte, indem Sie auf den Chevron klicken.

   ![Biometrische Geräte.](media/biometric-devices.png)

4. Ihr Fingerabdruckscanner sollte als biometrisches Gerät aufgeführt werden, z. B. der Synaptics WBDI-Scanner:

   ![Biometrische Geräte.](media/biometric-devices-expanded.png)

5. Wenn Ihr Fingerabdruckscanner nicht angezeigt wird und der Scanner in Ihren PC integriert ist, wechseln Sie zur Website des PC-Herstellers. Suchen Sie im Abschnitt technischer Support für Ihr PC-Modell nach einem Windows 10-Treiber für einen Scanner, den Sie installieren können.

6. Wenn der Scanner vom PC getrennt ist (über USB angeschlossen), wechseln Sie zur Website des Scannerherstellers, um die Windows 10-Gerätetreibersoftware für das Scannermodell zu finden und zu installieren.
