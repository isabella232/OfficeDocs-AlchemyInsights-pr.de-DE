---
title: Konfigurieren von Datenschutzeinstellungen in Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403860"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurieren von Datenschutzeinstellungen in Microsoft Edge

Wenn Microsoft Edge auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen standardmäßig nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch unter Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen entsprechend den [Windows-Diagnosedateneinstellungen der Benutzer gesendet.](https://go.microsoft.com/fwlink/?linkid=2132472)

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation verarbeitet:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiviert die Berichterstellung über Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sendet Websiteinformationen, die zur Verbesserung der Microsoft-Dienste verwendet werden.

Weitere Informationen finden Sie unter [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).
