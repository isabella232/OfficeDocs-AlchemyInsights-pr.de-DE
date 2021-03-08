---
title: Automatisches Verschieben von Nachrichten in das Archiv beenden
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522392"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="863eb-102">Automatisches Verschieben von Nachrichten in das Archiv beenden</span><span class="sxs-lookup"><span data-stu-id="863eb-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="863eb-103">Wenn Sie eine Aufbewahrungsrichtlinie verwenden, können Sie das Aufbewahrungszeitalter in dieser Richtlinie ändern, um zu verhindern, dass Nachrichten automatisch archiviert werden.</span><span class="sxs-lookup"><span data-stu-id="863eb-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="863eb-104">Dazu gehen Sie so vor:</span><span class="sxs-lookup"><span data-stu-id="863eb-104">Here's how:</span></span>

1. <span data-ttu-id="863eb-105">Wählen Sie [im Exchange Admin Center](https://go.microsoft.com/fwlink/?linkid=2059104) **Aufbewahrungstags für die**  >  **Complianceverwaltung aus.**</span><span class="sxs-lookup"><span data-stu-id="863eb-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="863eb-106">Suchen Sie nach dem Aufbewahrungstag "In Archiv verschieben".</span><span class="sxs-lookup"><span data-stu-id="863eb-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="863eb-107">Ändern Sie im Aufbewahrungstag den Aufbewahrungszeitraum (Archivzeitraum) in **Nie,** um zu verhindern, dass Elemente automatisch von einer Aufbewahrungsrichtlinie archiviert werden.</span><span class="sxs-lookup"><span data-stu-id="863eb-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="863eb-108">Dadurch wird die Archiveinstellung für alle Postfächer geändert, auf die dieses Aufbewahrungstag angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="863eb-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
