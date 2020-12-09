---
title: Microsoft Edge Konfigurieren von Datenschutzeinstellungen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599478"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge Konfigurieren von Datenschutzeinstellungen

Wenn Microsoft Edge standardmäßig auf nicht-Windows-Plattformen bereitgestellt wird, werden keine Diagnosedaten und Website Informationen an Microsoft gesendet. Wenn Microsoft Edge jedoch unter Windows 10 bereitgestellt wird, werden Diagnosedaten und Website Informationen entsprechend den [Windows-Diagnosedaten Einstellungen](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)von Benutzern gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie die Datensammlung für Ihre Organisation von Microsoft Edge verarbeitet wird:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Diese Richtlinie ermöglicht das Melden von Verwendungs-und Absturz bezogenen Daten.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Diese Richtlinie sendet Standortinformationen, die zur Verbesserung von Microsoft-Diensten verwendet werden.

Weitere Informationen finden Sie unter [configure Policy Settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).