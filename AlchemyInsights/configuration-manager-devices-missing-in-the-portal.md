---
title: Im-Portal fehlen Configuration Manager-Geräte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812150"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Im-Portal fehlen Configuration Manager-Geräte

Damit die Gerätesynchronisierung funktioniert, müssen die [erforderlichen Internet Endpunkte](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) über den lokalen Server erreichbar sein, auf dem die Rolle "Dienstverbindungspunkt" gehostet wird. Informationen zur Problembehandlung bei der Synchronisierung von Geräten finden Sie im **CMGatewaySyncUploadWorker.log**, das sich im Dienstverbindungspunkt befindet.

Erfahren Sie mehr über das [Anfügen von Mandanten in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
