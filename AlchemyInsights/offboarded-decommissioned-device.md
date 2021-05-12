---
title: Probleme beim Entfernen eines offboardierten oder außer Betrieb genommenen Geräts aus dem Gerätebestand
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319174"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="2bf9e-102">Probleme beim Entfernen eines offboardierten oder außer Betrieb genommenen Geräts aus dem Gerätebestand</span><span class="sxs-lookup"><span data-stu-id="2bf9e-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="2bf9e-103">Microsoft Defender for Endpoint lässt derzeit nicht zu, dass der Gerätedatensatz eines offboardierten oder außer Betrieb genommenen Geräts manuell aus dem Gerätebestand entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="2bf9e-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="2bf9e-104">Aus Sicherheitsgründen verbleibt das Gerät bis zu 180 Tage lang als historische Aufzeichnung im Portal.</span><span class="sxs-lookup"><span data-stu-id="2bf9e-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="2bf9e-105">Die Gerätedaten werden jedoch gemäß Dem konfigurierten Aufbewahrungszeitraum gelöscht.</span><span class="sxs-lookup"><span data-stu-id="2bf9e-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="2bf9e-106">**Hinweis:** Ein offboard- oder außer Betrieb genommenes Gerät wechselt nach sieben Tagen automatisch in den **Status Inaktiv.**</span><span class="sxs-lookup"><span data-stu-id="2bf9e-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="2bf9e-107">Darüber hinaus werden Geräte, die in den letzten 30 Tagen nicht aktiv waren, nicht in die Daten einbe berücksichtigt, die ihre Bedrohungs- und Sicherheitsrisikomanagement-Bewertung oder Microsoft Secure Score for Devices spiegeln.</span><span class="sxs-lookup"><span data-stu-id="2bf9e-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="2bf9e-108">Wenn bestimmte Geräte weiterhin nicht in der Geräteinventaransicht angezeigt werden möchten, versuchen Sie, ein Gerätetag zu platzieren, um das außer Betrieb genommene Gerät aus der Geräteinventaransicht heraus zu filtern.</span><span class="sxs-lookup"><span data-stu-id="2bf9e-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="2bf9e-109">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="2bf9e-109">For more information, see:</span></span>

[<span data-ttu-id="2bf9e-110">Offboardgeräte aus dem Microsoft Defender for Endpoint-Dienst</span><span class="sxs-lookup"><span data-stu-id="2bf9e-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="2bf9e-111">Gefährdungsergebnis im Bedrohungs- und Sicherheitsrisikomanagement</span><span class="sxs-lookup"><span data-stu-id="2bf9e-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="2bf9e-112">Beheben fehlerhafter Sensoren in Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="2bf9e-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="2bf9e-113">Effektive Verwendung von Tagging (Teil 1)</span><span class="sxs-lookup"><span data-stu-id="2bf9e-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="2bf9e-114">Effektive Verwendung von Tagging (Teil 2)</span><span class="sxs-lookup"><span data-stu-id="2bf9e-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="2bf9e-115">Effektive Verwendung von Tagging (Teil 3)</span><span class="sxs-lookup"><span data-stu-id="2bf9e-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




