---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770990"
---
# <a name="verify-your-domain"></a><span data-ttu-id="3edb7-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="3edb7-102">Verify your domain</span></span>

 <span data-ttu-id="3edb7-103">**Der Datensatz wurde wahrscheinlich nicht über das Internet aktualisiert.**</span><span class="sxs-lookup"><span data-stu-id="3edb7-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="3edb7-104">In der Regel dauert es nur ein paar Minuten, bis wir den neuen Eintrag sehen können, aber gelegentlich kann es auch ein paar Stunden dauern.</span><span class="sxs-lookup"><span data-stu-id="3edb7-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="3edb7-105">Wenn Sie so lange gewartet haben, überprüfen Sie, ob Sie den genauen Wert auf Ihrem DNS-Host kopiert und in den TXT-Überprüfungseintrag aufgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="3edb7-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="3edb7-106">Ein häufiges Problem ist, dass der Teil "MS=" des Eintrags fehlt.</span><span class="sxs-lookup"><span data-stu-id="3edb7-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="3edb7-107">Diese Angabe ist ebenfalls erforderlich!</span><span class="sxs-lookup"><span data-stu-id="3edb7-107">We need that too!</span></span>

- <span data-ttu-id="3edb7-108">Bei einigen DNS-Hosts müssen Sie einen zusätzlichen Schritt ausführen, um die Zonendatei zu speichern (in der der DNS-Eintrag gespeichert ist), damit der Eintrag im Internet aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="3edb7-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="3edb7-109">Stellen Sie sicher, dass Sie Ihre Änderungen gespeichert haben, damit Microsoft den Datensatz sehen und überprüfen kann.</span><span class="sxs-lookup"><span data-stu-id="3edb7-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
