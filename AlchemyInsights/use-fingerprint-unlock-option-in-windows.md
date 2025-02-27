---
title: Verwenden der Fingerabdruck-Entsperrungsoption in Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971902"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Verwenden der Fingerabdruck-Entsperrungsoption in Windows 10

**Aktivieren Windows Hello Fingerabdrucks**

Um Windows 10 mit ihrem Fingerabdruck zu entsperren, müssen Sie Windows Hello Fingerabdruck einrichten, indem Sie mindestens einen Finger hinzufügen (damit Windows lernen können, sie zu erkennen). 

1. Wechseln Sie zu **Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier).](ms-settings:signinoptions?activationSource=GetHelp) Verfügbare Anmeldeoptionen werden aufgelistet. Beispiel:

    ![Anmeldeoptionen.](media/sign-in-options.png)

2. Klicken oder tippen Sie **auf Windows Hello Fingerabdruck,** und klicken Sie dann auf **"Einrichten".** Klicken Sie im Windows Hello Setupfenster auf **"Erste Schritte".** Der Fingerabdrucksensor wird aktiviert, und Sie werden aufgefordert, Ihren Finger auf den Sensor zu platzieren:

   ![Fingerabdrucksensor.](media/fingerprint-sensor.png)

3. Folgen Sie den Anweisungen, in denen Sie aufgefordert werden, wiederholt mit dem Finger zu scannen. Nach Abschluss dieses Vorgangs haben Sie die Möglichkeit, weitere Finger hinzuzufügen, die Sie für die Anmeldung verwenden möchten. Wenn Sie sich das nächste Mal bei Windows 10 anmelden, haben Sie die Möglichkeit, dazu Ihren Fingerabdruck zu verwenden.

**Windows Hello Fingerabdruck nicht als Anmeldeoption verfügbar**

Wenn Windows Hello Fingerabdruck nicht als Option in **den Anmeldeoptionen** angezeigt wird, bedeutet dies, dass Windows keinen Fingerabdruckleser/Scanner erkennt, der an Ihren PC angefügt ist, oder dass eine Systemrichtlinie die Verwendung verhindert (z. B. wenn Ihr PC von Ihrem Arbeitsplatz verwaltet wird). So beheben Sie Probleme: 

1. Wählen Sie die **Startschaltfläche** in der Taskleiste aus, und suchen Sie nach **Device Manager.**

2. Klicken oder tippen Sie, um den **Geräte-Manager** zu öffnen.

3. Erweitern Sie im Geräte-Manager biometrische Geräte, indem Sie auf das zugehörige Chevron klicken.

   ![Biometrische Geräte.](media/biometric-devices.png)

4. Ihr Fingerabdruckscanner sollte als biometrisches Gerät, z. B. der Synaptics WBDI-Scanner, aufgeführt werden:

   ![Biometrische Geräte.](media/biometric-devices-expanded.png)

5. Wenn Ihr Fingerabdruckscanner nicht angezeigt wird und der Scanner in Ihren PC integriert ist, wechseln Sie zur Website des PC-Herstellers. Suchen Sie im Abschnitt "Technischer Support" für Ihr PC-Modell nach einem Windows 10 Treiber für einen Scanner, den Sie installieren können.

6. Wenn der Scanner vom PC getrennt ist (über USB angeschlossen), wechseln Sie zur Website des Scannerherstellers, um Windows 10 Gerätetreibersoftware für das Scannermodell zu suchen und zu installieren.
