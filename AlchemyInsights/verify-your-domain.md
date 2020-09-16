---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734305"
---
# <a name="verify-your-domain"></a><span data-ttu-id="6e9c5-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="6e9c5-102">Verify your domain</span></span>

 <span data-ttu-id="6e9c5-103">**Der Datensatz wurde möglicherweise nicht über das Internet aktualisiert.**</span><span class="sxs-lookup"><span data-stu-id="6e9c5-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="6e9c5-104">In der Regel dauert es nur ein paar Minuten, bis wir den neuen Eintrag sehen können, aber gelegentlich kann es auch ein paar Stunden dauern.</span><span class="sxs-lookup"><span data-stu-id="6e9c5-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="6e9c5-105">Wenn Sie schon so lange gewartet haben, überprüfen Sie, ob Sie den exakten Wert kopiert und in den txt-Überprüfungs Eintrag auf Ihrem DNS-Host eingefügt haben.</span><span class="sxs-lookup"><span data-stu-id="6e9c5-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="6e9c5-106">Ein häufiges Problem ist, dass der Teil "MS=" des Eintrags fehlt.</span><span class="sxs-lookup"><span data-stu-id="6e9c5-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="6e9c5-107">Diese Angabe ist ebenfalls erforderlich!</span><span class="sxs-lookup"><span data-stu-id="6e9c5-107">We need that too!</span></span>

- <span data-ttu-id="6e9c5-108">Bei einigen DNS-Hosts müssen Sie einen zusätzlichen Schritt ausführen, um die Zonendatei zu speichern (in der der DNS-Eintrag gespeichert ist), damit der Eintrag im Internet aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="6e9c5-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="6e9c5-109">Stellen Sie sicher, dass Sie Ihre Änderungen gespeichert haben, damit Microsoft den Datensatz sehen und überprüfen kann.</span><span class="sxs-lookup"><span data-stu-id="6e9c5-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
