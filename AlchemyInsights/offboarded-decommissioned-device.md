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
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Probleme beim Entfernen eines offboardierten oder außer Betrieb genommenen Geräts aus dem Gerätebestand

Microsoft Defender for Endpoint lässt derzeit nicht zu, dass der Gerätedatensatz eines offboardierten oder außer Betrieb genommenen Geräts manuell aus dem Gerätebestand entfernt wird.

Aus Sicherheitsgründen verbleibt das Gerät bis zu 180 Tage lang als historische Aufzeichnung im Portal. Die Gerätedaten werden jedoch gemäß Dem konfigurierten Aufbewahrungszeitraum gelöscht.

**Hinweis:** Ein offboard- oder außer Betrieb genommenes Gerät wechselt nach sieben Tagen automatisch in den **Status Inaktiv.** Darüber hinaus werden Geräte, die in den letzten 30 Tagen nicht aktiv waren, nicht in die Daten einbe berücksichtigt, die ihre Bedrohungs- und Sicherheitsrisikomanagement-Bewertung oder Microsoft Secure Score for Devices spiegeln.
 
Wenn bestimmte Geräte weiterhin nicht in der Geräteinventaransicht angezeigt werden möchten, versuchen Sie, ein Gerätetag zu platzieren, um das außer Betrieb genommene Gerät aus der Geräteinventaransicht heraus zu filtern.

Weitere Informationen finden Sie unter:

[Offboardgeräte aus dem Microsoft Defender for Endpoint-Dienst](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Gefährdungsergebnis im Bedrohungs- und Sicherheitsrisikomanagement](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Beheben fehlerhafter Sensoren in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Effektive Verwendung von Tagging (Teil 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Effektive Verwendung von Tagging (Teil 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Effektive Verwendung von Tagging (Teil 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




