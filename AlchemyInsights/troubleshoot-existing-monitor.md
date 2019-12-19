---
title: Problembehandlung für vorhandenen Monitor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738568"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="015a9-102">Problembehandlung bei einem vorhandenen Monitor</span><span class="sxs-lookup"><span data-stu-id="015a9-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="015a9-103">Versuchen Sie diese Lösungen zur Problembehandlung für einen Monitor.</span><span class="sxs-lookup"><span data-stu-id="015a9-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="015a9-104">**Aktualisieren Sie die Anzeige Ihres Monitors:**</span><span class="sxs-lookup"><span data-stu-id="015a9-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="015a9-105">Drücken Sie gleichzeitig die folgenden Tasten: Windows-Taste + STRG + UMSCHALT + B. Dadurch wird die Kommunikation mit Ihrem Grafiktreiber aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="015a9-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="015a9-106">Ihre Monitore blinken kurz und kommen nach ein paar Sekunden zurück.</span><span class="sxs-lookup"><span data-stu-id="015a9-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="015a9-107">**Problembehandlung bei der Hardwareüberwachung:**</span><span class="sxs-lookup"><span data-stu-id="015a9-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="015a9-108">Ziehen Sie das Kabel, das Ihren PC mit dem Monitor verbindet, aus, und stecken Sie es wieder ein.</span><span class="sxs-lookup"><span data-stu-id="015a9-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="015a9-109">Trennen Sie alle nicht wesentlichen Geräte von Ihrem PC (wie Adapter oder Docks).</span><span class="sxs-lookup"><span data-stu-id="015a9-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="015a9-110">**Wenn Sie vor kurzem ein Update auf Ihrem PC installiert haben, können Sie den Bildschirmtreiber wiederherstellen:**</span><span class="sxs-lookup"><span data-stu-id="015a9-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="015a9-111">Wählen Sie **Start**, geben Sie **Geräte-Manager**ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="015a9-112">Erweitern Sie den Abschnitt **Anzeigeadapter** , klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Eigenschaften**aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="015a9-113">Navigieren Sie zur Registerkarte **Treiber** , und wählen Sie **Rollback Driver**aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="015a9-114">Hinweis: Wenn diese Option nicht verfügbar ist oder abgeblendet ist, wählen Sie in den Optionen unten die Option **Nein** aus, um zum nächsten Schritt zu gelangen.</span><span class="sxs-lookup"><span data-stu-id="015a9-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="015a9-115">Möglicherweise müssen Sie Ihren PC neu starten, bevor diese Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="015a9-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="015a9-116">**Deinstallieren Sie den Anzeigetreiber, und installieren Sie ihn neu:**</span><span class="sxs-lookup"><span data-stu-id="015a9-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="015a9-117">Wählen Sie **Start**, geben Sie **Geräte-Manager**ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="015a9-118">Erweitern Sie den Abschnitt **Anzeigeadapter** , klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Gerät deinstallieren**aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="015a9-119">Aktivieren Sie das Kontrollkästchen neben **die Treibersoftware für dieses Gerät löschen** , und wählen Sie **deinstallieren**aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="015a9-120">Hinweis: Sie werden möglicherweise aufgefordert, Ihren Computer zu diesem Zeitpunkt neu zu starten.</span><span class="sxs-lookup"><span data-stu-id="015a9-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="015a9-121">Achten Sie darauf, dass Sie die restlichen Anweisungen vor dem Neustart notieren.</span><span class="sxs-lookup"><span data-stu-id="015a9-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="015a9-122">Öffnen Sie erneut den Geräte-Manager.</span><span class="sxs-lookup"><span data-stu-id="015a9-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="015a9-123">Erweitern Sie den Abschnitt **Anzeigeadapter** , klicken Sie mit der rechten Maustaste auf Ihren Anzeigeadapter, und wählen Sie **Treiber aktualisieren**aus.</span><span class="sxs-lookup"><span data-stu-id="015a9-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="015a9-124">Wählen Sie **Automatische Suche für Update Treibersoftware** aus, und befolgen Sie die Installationsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="015a9-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>