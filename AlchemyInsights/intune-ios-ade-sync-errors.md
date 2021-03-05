---
title: Synchronisierungsfehler bei der automatischen Geräteregistrierung bei Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448921"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synchronisierungsfehler bei der automatischen Geräteregistrierung bei Apple

"Wir haben festgestellt, dass Sie über ein oder mehrere ADE/DEP-Token verfügen, die sich im Fehlerzustand befinden. Bis der Fehlerstatus für jedes betroffene Token aufgelöst wurde, funktioniert die ADE-Funktion nicht wie erwartet."

Dieser Fehler kann auf verschiedene Weise manifestiert werden, z. B.:

1. Geräte werden möglicherweise nicht von ABM/ASM mit Intune synchronisiert
2. Registrierungsprofilzuweisungen können fehlgeschlagen sein
3. Geräte können die ADE-Registrierung möglicherweise nicht erfolgreich abschließen

Überprüfen Sie auf den Synchronisierungsfehler, der in der Intune-Konsole unter Geräte > Registrieren von Geräten > Registrierung von Apple > **Registrierungsprogrammtoken gemeldet wurde.**

Eine der häufigsten Ursachen für Synchronisierungsfehler ist das Ablaufen des aktuellen Tokens. In vielen Fällen wird das Problem durch die Verlängerung des betroffenen Tokens behoben.

Wenn eines oder mehrere Ihrer Token abgelaufen sind, lesen Sie die folgende Dokumentation, um sie gegebenenfalls zu verlängern:

[Verlängern eines Tokens für die automatische Geräteregistrierung](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Darüber hinaus sehen Sie in der folgenden Dokumentation mögliche Korrekturen für andere Fehler, die zu Fehlern bei der Tokensynchronisierung führen:

[ABM-/ASM-Synchronisierungsfehler für iOS/iPadOS- und macOS-Token für die automatische Geräteregistrierung](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM-/ASM-Synchronisierungsfehler für iOS/iPadOS- und macOS-Token für die automatische Geräteregistrierung](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
