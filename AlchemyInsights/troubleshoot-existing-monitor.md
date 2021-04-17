---
title: Problembehandlung bei vorhandenen Monitoren
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824578"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="93e0d-102">Problembehandlung für einen vorhandenen Monitor</span><span class="sxs-lookup"><span data-stu-id="93e0d-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="93e0d-103">Probieren Sie diese Lösungen aus, um probleme mit einem Monitor zu beheben.</span><span class="sxs-lookup"><span data-stu-id="93e0d-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="93e0d-104">**Aktualisieren sie die Anzeige Ihres Monitors:**</span><span class="sxs-lookup"><span data-stu-id="93e0d-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="93e0d-105">Drücken Sie die folgenden Tasten gleichzeitig: Windows-TASTE + STRG + Umschalt + B. Dadurch wird die Kommunikation mit dem Grafiktreiber aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="93e0d-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="93e0d-106">Ihre Monitore blinken kurz und kommen nach ein paar Sekunden zurück.</span><span class="sxs-lookup"><span data-stu-id="93e0d-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="93e0d-107">**Problembehandlung bei der Monitorhardware:**</span><span class="sxs-lookup"><span data-stu-id="93e0d-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="93e0d-108">Ziehen Sie das Kabel ab, das Ihren PC mit Ihrem Monitor verbindet, und schließen Sie es wieder an.</span><span class="sxs-lookup"><span data-stu-id="93e0d-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="93e0d-109">Trennen Sie alle nicht wesentlichen Geräte von Ihrem PC (z. B. Adapter oder Dockingstationen).</span><span class="sxs-lookup"><span data-stu-id="93e0d-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="93e0d-110">**Wenn Sie kürzlich ein Update auf Ihrem PC installiert haben, können Sie ein Rollback des Anzeigetreibers starten:**</span><span class="sxs-lookup"><span data-stu-id="93e0d-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="93e0d-111">Wählen **Sie Start** aus, geben Sie **Geräte-Manager** ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.</span><span class="sxs-lookup"><span data-stu-id="93e0d-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="93e0d-112">Erweitern Sie **den Abschnitt Anzeigeadapter,** klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Eigenschaften aus.**</span><span class="sxs-lookup"><span data-stu-id="93e0d-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="93e0d-113">Navigieren Sie zur **Registerkarte Treiber,** und wählen Sie **Roll Back Driver aus.**</span><span class="sxs-lookup"><span data-stu-id="93e0d-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="93e0d-114">Hinweis: Wenn dies nicht verfügbar ist oder  ausgegraut ist, wählen Sie in den folgenden Optionen Nein aus, um zum nächsten Schritt zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="93e0d-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="93e0d-115">Möglicherweise müssen Sie Ihren PC neu starten, bevor diese Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="93e0d-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="93e0d-116">**Deinstallieren und installieren Sie den Anzeigetreiber:**</span><span class="sxs-lookup"><span data-stu-id="93e0d-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="93e0d-117">Wählen **Sie Start** aus, geben Sie **Geräte-Manager** ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.</span><span class="sxs-lookup"><span data-stu-id="93e0d-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="93e0d-118">Erweitern Sie **den Abschnitt Anzeigeadapter,** klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Gerät deinstallieren aus.**</span><span class="sxs-lookup"><span data-stu-id="93e0d-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="93e0d-119">Wählen Sie das Feld neben **Treibersoftware für dieses Gerät löschen aus,** und wählen Sie **Deinstallieren aus.**</span><span class="sxs-lookup"><span data-stu-id="93e0d-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="93e0d-120">Hinweis: Sie werden möglicherweise aufgefordert, Ihren Computer zu diesem Zeitpunkt neu zu starten.</span><span class="sxs-lookup"><span data-stu-id="93e0d-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="93e0d-121">Notieren Sie sich vor dem Neustart unbedingt die restlichen Anweisungen.</span><span class="sxs-lookup"><span data-stu-id="93e0d-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="93e0d-122">Öffnen Sie den Geräte-Manager erneut.</span><span class="sxs-lookup"><span data-stu-id="93e0d-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="93e0d-123">Erweitern Sie **den Abschnitt Adapter anzeigen,** klicken Sie mit der rechten Maustaste auf den Anzeigeadapter, und wählen Sie **Treiber aktualisieren aus.**</span><span class="sxs-lookup"><span data-stu-id="93e0d-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="93e0d-124">Wählen **Sie Automatisch nach Updatetreibersoftware suchen aus,** und befolgen Sie die Installationsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="93e0d-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>