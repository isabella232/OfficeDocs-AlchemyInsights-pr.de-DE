---
title: Auffinden verlorener iOS-Geräte mit Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434594"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="ff813-102">Auffinden verlorener iOS-Geräte mit Intune</span><span class="sxs-lookup"><span data-stu-id="ff813-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="ff813-103">Wenn Sie den Modus für verlorene Geräte auf einem iOS-Gerät aktivieren, kann einem Administrator auf dem Sperrbildschirm eine Nachricht und eine Kontakttelefonnummer angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ff813-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="ff813-104">Nachdem der Modus für verlorene Geräte aktiviert wurde, kann der Administrator die Aktion „Gerät suchen“ verwenden, um den physischen Standort des Geräts zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="ff813-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="ff813-105">Die Aktion „Gerät suchen“ in Intune funktioniert mit iOS-Geräten, um den Standort eines bestimmten Geräts auf einer Karte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="ff813-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="ff813-106">Damit diese Aktion verwendet werden kann, muss sich das iOS-Gerät in einem der folgenden Modi befinden:</span><span class="sxs-lookup"><span data-stu-id="ff813-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="ff813-107">Überwachter Modus</span><span class="sxs-lookup"><span data-stu-id="ff813-107">Supervised mode</span></span>
- <span data-ttu-id="ff813-108">Modus für verlorene Geräte</span><span class="sxs-lookup"><span data-stu-id="ff813-108">Lost mode</span></span>

<span data-ttu-id="ff813-109">Weitere Informationen hierzu finden Sie unter [Aktivieren des Modus für verlorene Geräte auf iOS-/iPad-Geräten mit Intune](https://docs.microsoft.com/intune/device-lost-mode) und [Auffinden verlorener oder gestohlener iOS-/iPad-Geräte mit Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="ff813-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="ff813-110">**Häufig gestellte Fragen**</span><span class="sxs-lookup"><span data-stu-id="ff813-110">**FAQ**</span></span>

<span data-ttu-id="ff813-111">F: Ich habe eine Remoteaktion zum Entfernen von Unternehmensdaten von einem Gerät gesendet, und jetzt ist das Gerät im Zustand „Ausstehend“ hängen geblieben.</span><span class="sxs-lookup"><span data-stu-id="ff813-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="ff813-112">A: Damit eine Remoteaktion erfolgreich abgeschlossen werden kann, muss das Zielgerät online und fehlerfrei sein.</span><span class="sxs-lookup"><span data-stu-id="ff813-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="ff813-113">In den folgenden Situationen bleibt die Remoteaktion 30 Tage lang im Zustand „Ausstehend“ oder bis das Gerät den Befehl bestätigt:</span><span class="sxs-lookup"><span data-stu-id="ff813-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="ff813-114">Wenn das Gerät keine Verbindung hat.</span><span class="sxs-lookup"><span data-stu-id="ff813-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="ff813-115">Wenn das Gerät seinen Verwaltungsstatus bei Intune verloren hat.</span><span class="sxs-lookup"><span data-stu-id="ff813-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="ff813-116">Wenn Sie der Meinung sind, dass das Gerät keinen Check-In mehr vornimmt und dass es nicht mehr in der Lage ist, Unternehmensdaten zu entfernen, wählen Sie „Löschen“ aus.</span><span class="sxs-lookup"><span data-stu-id="ff813-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="ff813-117">Durch das Löschen wird der Gerätedatensatz entfernt, sodass er nicht mehr in der Liste der Geräte in Intune angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ff813-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="ff813-118">Wenn das Gerät wieder aktiv wird, muss sein Benutzer es erneut registrieren.</span><span class="sxs-lookup"><span data-stu-id="ff813-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="ff813-119">F: Warum sind bestimmte Remoteaktionen für mich nicht verfügbar?</span><span class="sxs-lookup"><span data-stu-id="ff813-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="ff813-120">A: Nicht alle Plattformen unterstützen alle Remoteaktionen für Geräte.</span><span class="sxs-lookup"><span data-stu-id="ff813-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="ff813-121">Die folgenden Remoteaktionen sind plattformspezifisch, sodass Sie nur für die aufgeführten Plattformen verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="ff813-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="ff813-122">Aktivierungssperre umgehen (nur iOS)</span><span class="sxs-lookup"><span data-stu-id="ff813-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="ff813-123">Sauberer Start (nur Windows)</span><span class="sxs-lookup"><span data-stu-id="ff813-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="ff813-124">Modus für verlorene Geräte (nur iOS)</span><span class="sxs-lookup"><span data-stu-id="ff813-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="ff813-125">Gerät suchen (nur iOS)</span><span class="sxs-lookup"><span data-stu-id="ff813-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="ff813-126">Neustart (nur Windows)</span><span class="sxs-lookup"><span data-stu-id="ff813-126">Restart (Windows only)</span></span>

<span data-ttu-id="ff813-127">Weitere Details zu den einzelnen Aktionen finden Sie unter [Verfügbare Geräteaktionen](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="ff813-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>