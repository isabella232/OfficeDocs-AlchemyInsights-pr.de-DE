---
title: Beheben von Transportregeln
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
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737135"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="1f635-102">Beheben von Transportregeln</span><span class="sxs-lookup"><span data-stu-id="1f635-102">Fix transport rules</span></span>

<span data-ttu-id="1f635-103">Diese Nachricht wurde von einer benutzerdefinierten Nachrichtenflussregel beeinflusst.</span><span class="sxs-lookup"><span data-stu-id="1f635-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="1f635-104">Gehen Sie wie folgt vor, um die genaue Regel zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="1f635-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="1f635-105">Notieren Sie sich in den Übermittlungsergebnissen unter **Zusätzliche Informationen** die **GUID** oder **den Richtliniennamen**.</span><span class="sxs-lookup"><span data-stu-id="1f635-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="1f635-106">Starten Sie die Exchange-Verwaltungsshell.</span><span class="sxs-lookup"><span data-stu-id="1f635-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="1f635-107">Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="1f635-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="1f635-108">Führen Sie diesen Befehl aus (mithilfe der GUID aus Ihrer Übermittlung):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="1f635-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="1f635-109">Überprüfen Sie die Beschreibung, um die konfigurierten Bedingungen zu sehen, die sich auf die Nachricht ausdrückten.</span><span class="sxs-lookup"><span data-stu-id="1f635-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="1f635-110">Weitere Informationen finden Sie unter [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="1f635-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
