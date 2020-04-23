---
title: Im-Portal fehlen Configuration Manager-Geräte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789901"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="34e4f-102">Im-Portal fehlen Configuration Manager-Geräte</span><span class="sxs-lookup"><span data-stu-id="34e4f-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="34e4f-103">Damit die Gerätesynchronisierung funktioniert, müssen die [erforderlichen Internet Endpunkte](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) über den lokalen Server erreichbar sein, auf dem die Rolle "Dienstverbindungspunkt" gehostet wird.</span><span class="sxs-lookup"><span data-stu-id="34e4f-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="34e4f-104">Informationen zur Problembehandlung bei der Synchronisierung von Geräten finden Sie im **CMGatewaySyncUploadWorker.log**, das sich im Dienstverbindungspunkt befindet.</span><span class="sxs-lookup"><span data-stu-id="34e4f-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="34e4f-105">Erfahren Sie mehr über das [Anfügen von Mandanten in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="34e4f-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
