---
title: Doppelter Gerätedatensatz im Portal
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
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678503"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="14af3-102">Doppelter Gerätedatensatz im Portal</span><span class="sxs-lookup"><span data-stu-id="14af3-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="14af3-103">Sie sehen möglicherweise zwei Datensätze für ein Gerät im Portal, wenn das Gerät den Co-Verwaltungsstatus nicht korrekt an die Configuration-Manager-Site meldet.</span><span class="sxs-lookup"><span data-stu-id="14af3-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="14af3-104">Um den Co-Verwaltungsstatus eines Geräts zu überprüfen, überprüfen Sie die Spalte **Co-verwaltet** auf das Gerät in der Configuration Manager-Konsole.</span><span class="sxs-lookup"><span data-stu-id="14af3-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="14af3-105">Wenn die Spalte nicht sichtbar ist, können Sie sie hinzufügen, indem Sie mit der rechten Maustaste auf eine der Spaltenüberschriften klicken und sie aus der Liste auswählen.</span><span class="sxs-lookup"><span data-stu-id="14af3-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="14af3-106">Der Wert für „Co-verwaltet“ muss **Ja** lauten.</span><span class="sxs-lookup"><span data-stu-id="14af3-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="14af3-107">Wenn der Wert **Nein** lautet, öffnen Sie das Configuration Manager-Client-Applet auf dem Client-Gerät, und aktivieren Sie die Eigenschaft **Co-Verwaltung** auf der Registerkarte „Allgemein“.</span><span class="sxs-lookup"><span data-stu-id="14af3-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="14af3-108">Wenn der Wert **Aktiviert** lautet, bedeutet dies, dass es Probleme mit der Kommunikation des Clients mit dem Verwaltungspunkt gibt.</span><span class="sxs-lookup"><span data-stu-id="14af3-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="14af3-109">Bitte lesen Sie auf dem Gerät die Datei **CcmMessaging.log** durch, um mögliche Verbindungsprobleme zu untersuchen.</span><span class="sxs-lookup"><span data-stu-id="14af3-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="14af3-110">Wenn der Wert **Deaktiviert** lautet und das Gerät bei Intune angemeldet ist, stellen Sie bitte sicher, dass das Gerät die Co-Verwaltungsrichtlinie erhalten hat, indem Sie die Datei **CoManagementHandler.log** auf dem Gerät überprüfen.</span><span class="sxs-lookup"><span data-stu-id="14af3-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
