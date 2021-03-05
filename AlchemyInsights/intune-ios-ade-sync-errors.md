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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="4d6d4-102">Synchronisierungsfehler bei der automatischen Geräteregistrierung bei Apple</span><span class="sxs-lookup"><span data-stu-id="4d6d4-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="4d6d4-103">"Wir haben festgestellt, dass Sie über ein oder mehrere ADE/DEP-Token verfügen, die sich im Fehlerzustand befinden.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="4d6d4-104">Bis der Fehlerstatus für jedes betroffene Token aufgelöst wurde, funktioniert die ADE-Funktion nicht wie erwartet."</span><span class="sxs-lookup"><span data-stu-id="4d6d4-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="4d6d4-105">Dieser Fehler kann auf verschiedene Weise manifestiert werden, z. B.:</span><span class="sxs-lookup"><span data-stu-id="4d6d4-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="4d6d4-106">Geräte werden möglicherweise nicht von ABM/ASM mit Intune synchronisiert</span><span class="sxs-lookup"><span data-stu-id="4d6d4-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="4d6d4-107">Registrierungsprofilzuweisungen können fehlgeschlagen sein</span><span class="sxs-lookup"><span data-stu-id="4d6d4-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="4d6d4-108">Geräte können die ADE-Registrierung möglicherweise nicht erfolgreich abschließen</span><span class="sxs-lookup"><span data-stu-id="4d6d4-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="4d6d4-109">Überprüfen Sie auf den Synchronisierungsfehler, der in der Intune-Konsole unter Geräte > Registrieren von Geräten > Registrierung von Apple > **Registrierungsprogrammtoken gemeldet wurde.**</span><span class="sxs-lookup"><span data-stu-id="4d6d4-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="4d6d4-110">Eine der häufigsten Ursachen für Synchronisierungsfehler ist das Ablaufen des aktuellen Tokens.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="4d6d4-111">In vielen Fällen wird das Problem durch die Verlängerung des betroffenen Tokens behoben.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="4d6d4-112">Wenn eines oder mehrere Ihrer Token abgelaufen sind, lesen Sie die folgende Dokumentation, um sie gegebenenfalls zu verlängern:</span><span class="sxs-lookup"><span data-stu-id="4d6d4-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="4d6d4-113">Verlängern eines Tokens für die automatische Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="4d6d4-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="4d6d4-114">Darüber hinaus sehen Sie in der folgenden Dokumentation mögliche Korrekturen für andere Fehler, die zu Fehlern bei der Tokensynchronisierung führen:</span><span class="sxs-lookup"><span data-stu-id="4d6d4-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="4d6d4-115">ABM-/ASM-Synchronisierungsfehler für iOS/iPadOS- und macOS-Token für die automatische Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="4d6d4-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="4d6d4-116">ABM-/ASM-Synchronisierungsfehler für iOS/iPadOS- und macOS-Token für die automatische Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="4d6d4-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
