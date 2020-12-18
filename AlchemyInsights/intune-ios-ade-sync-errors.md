---
title: Synchronisierungsfehler bei Apple für die automatische Geräteregistrierung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707894"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synchronisierungsfehler bei Apple für die automatische Geräteregistrierung

"Wir haben festgestellt, dass Sie über mindestens ein ADE/DEP-Token verfügen, das einen Fehlerzustand aufweist. Bis der Fehlerzustand für jedes betroffene Token aufgelöst wird, funktioniert die ADE-Funktion nicht für die gleiche ".

Dieser Fehler kann sich auf verschiedene Weise manifestieren, einschließlich:

1. Geräte dürfen nicht von ABM/ASM zu InTune synchronisiert werden
2. Bei Registrierungsprofil Zuweisungen kann ein Fehler auftreten
3. Bei Geräten ist die ADE-Registrierung möglicherweise nicht erfolgreich abgeschlossen.

Überprüfen Sie den in der InTune-Konsole gemeldeten Synchronisierungsfehler unter **Geräte > Geräte registrieren > Apple Enrollment > Registrierungsprogramm Tokens** , und lesen Sie die folgende Dokumentation, um mögliche Korrekturen anzuzeigen:

[ABM/ASM-Synchronisierungsfehler für IOS/iPad-und macOS-automatische Geräte Registrierungstoken](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
