---
title: Port Google Chrome Extensions to Microsoft Edge (Chrom)
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
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600113"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port Google Chrome Extensions to Microsoft Edge (Chrom)

Es ist ganz einfach, [Google Chrome-Erweiterungen an Microsoft Edge (Chrom) zu portieren](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). In den meisten Fällen sind nur minimale Änderungen erforderlich, um diese Erweiterungen auf Microsoft Edge auszuführen.

Die von Google Chrome unterstützten Erweiterungs-APIs und manifestschlüssel sind mit Microsoft Edge Code kompatibel. Microsoft Edge unterstützt jedoch nicht die Erweiterungs-APIs "Chrome. GCM", "Chrome. Identity. getaccounts", "Chrome. Identity. getAuthToken" und "Chrome. InstanceId".