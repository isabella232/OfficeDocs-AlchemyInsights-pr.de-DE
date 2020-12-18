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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="14abc-102">Synchronisierungsfehler bei Apple für die automatische Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="14abc-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="14abc-103">"Wir haben festgestellt, dass Sie über mindestens ein ADE/DEP-Token verfügen, das einen Fehlerzustand aufweist.</span><span class="sxs-lookup"><span data-stu-id="14abc-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="14abc-104">Bis der Fehlerzustand für jedes betroffene Token aufgelöst wird, funktioniert die ADE-Funktion nicht für die gleiche ".</span><span class="sxs-lookup"><span data-stu-id="14abc-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="14abc-105">Dieser Fehler kann sich auf verschiedene Weise manifestieren, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="14abc-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="14abc-106">Geräte dürfen nicht von ABM/ASM zu InTune synchronisiert werden</span><span class="sxs-lookup"><span data-stu-id="14abc-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="14abc-107">Bei Registrierungsprofil Zuweisungen kann ein Fehler auftreten</span><span class="sxs-lookup"><span data-stu-id="14abc-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="14abc-108">Bei Geräten ist die ADE-Registrierung möglicherweise nicht erfolgreich abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="14abc-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="14abc-109">Überprüfen Sie den in der InTune-Konsole gemeldeten Synchronisierungsfehler unter **Geräte > Geräte registrieren > Apple Enrollment > Registrierungsprogramm Tokens** , und lesen Sie die folgende Dokumentation, um mögliche Korrekturen anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="14abc-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="14abc-110">ABM/ASM-Synchronisierungsfehler für IOS/iPad-und macOS-automatische Geräte Registrierungstoken</span><span class="sxs-lookup"><span data-stu-id="14abc-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
