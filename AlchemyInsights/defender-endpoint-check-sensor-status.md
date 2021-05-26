---
title: Defender-Endpunkt – Überprüfen Sie den Sensorstatus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627245"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="eece2-102">Defender-Endpunkt – Überprüfen Sie den Sensorstatus</span><span class="sxs-lookup"><span data-stu-id="eece2-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="eece2-103">Die Kachel **Geräte mit Sensorproblemen** befindet sich auf dem Dashboard "Sicherheitsvorgänge".</span><span class="sxs-lookup"><span data-stu-id="eece2-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="eece2-104">Diese Kachel enthält Informationen über die Kapazität des einzelnen Geräts, Sensordaten zu liefern und mit dem Defender für Endpunkt-Dienst zu kommunizieren.</span><span class="sxs-lookup"><span data-stu-id="eece2-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="eece2-105">Sie zeigt an, wie viele Geräte Ihrer Aufmerksamkeit erfordern und hilft Ihnen, problematische Geräte zu identifizieren und Maßnahmen zur Behebung bekannter Probleme zu ergreifen.</span><span class="sxs-lookup"><span data-stu-id="eece2-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="eece2-106">Zwei Statusindikatoren auf der Kachel enthalten Informationen zur Anzahl der Geräte, die nicht ordnungsgemäß an den Dienst gemeldet werden:</span><span class="sxs-lookup"><span data-stu-id="eece2-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="eece2-107">**Falsch konfigurierte** Geräte, die sensorische Daten möglicherweise nur teilweise beim Defender für Endpunkt-Dienst melden bzw. Konfigurationsfehler haben, die behoben werden müssen.</span><span class="sxs-lookup"><span data-stu-id="eece2-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="eece2-108">**Inaktive** Geräte, die seit mehr als sieben Tagen im letzten Monat keine Meldungen mehr an den Defender für Endpunkt-Dienst gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="eece2-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="eece2-109">Wenn Sie auf eine der Gruppen klicken, werden Sie zur Liste "Geräte" umgeleitet, die entsprechend Ihrer Auswahl gefiltert ist.</span><span class="sxs-lookup"><span data-stu-id="eece2-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="eece2-110">In der Liste "Geräte" können Sie die Liste des Integritätsstatus nach dem folgenden Status filtern:</span><span class="sxs-lookup"><span data-stu-id="eece2-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="eece2-111">**Aktive** Geräte, die aktiv Meldungen an den Defender für Endpunkt-Dienst senden.</span><span class="sxs-lookup"><span data-stu-id="eece2-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="eece2-112">**Falsch konfigurierte** Geräte, die sensorische Daten möglicherweise nur teilweise beim Defender für Endpunkt-Dienst melden, die jedoch Konfigurationsfehler haben, die behoben werden müssen.</span><span class="sxs-lookup"><span data-stu-id="eece2-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="eece2-113">Falsch konfigurierte Geräte können entweder eins oder eine Mischung aus den folgenden Probleme haben:</span><span class="sxs-lookup"><span data-stu-id="eece2-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="eece2-114">Keine Sensordaten – Die Geräte haben aufgehört, Sensordaten zu senden.</span><span class="sxs-lookup"><span data-stu-id="eece2-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="eece2-115">Das Gerät kann begrenzt Alarme auslösen.</span><span class="sxs-lookup"><span data-stu-id="eece2-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="eece2-116">Eingeschränkte Kommunikation – Die Kommunikation mit dem Gerät ist beeinträchtigt.</span><span class="sxs-lookup"><span data-stu-id="eece2-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="eece2-117">Dateien zur tiefen Analyse senden, Dateien sperren, das Gerät vom Netzwerk isolieren und andere Aktionen, die eine Kommunikation mit dem Gerät erfordern, funktionieren möglicherweise nicht.</span><span class="sxs-lookup"><span data-stu-id="eece2-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="eece2-118">**Inaktive** Geräte, die keine Meldungen an den Defender für Endpunkt-Dienst mehr senden.</span><span class="sxs-lookup"><span data-stu-id="eece2-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="eece2-119">Sie können die gesamte Liste im CSV-Format mithilfe der Exportfunktion herunterladen.</span><span class="sxs-lookup"><span data-stu-id="eece2-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="eece2-120">Weitere Informationen finden Sie unter [Überprüfen des Integritätsstatus des Sensor in Microsoft Defender für Endpunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="eece2-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="eece2-121">Weitere Informationen darüber, was dazu geführt hat, dass ein Gerät inaktiv oder falsch konfiguriert war, finden Sie unter [Beheben fehlerhafter Sensoren in Microsoft Defender für Endpunkt](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="eece2-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
