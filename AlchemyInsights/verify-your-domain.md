---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d215f3af0cf4b46b12c8cb51a9572adb00f354e4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420051"
---
# <a name="verify-your-domain"></a><span data-ttu-id="bf3a3-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="bf3a3-102">Verify your domain</span></span>

 <span data-ttu-id="bf3a3-103">**Der Datensatz wurde wahrscheinlich nicht über das Internet aktualisiert.**</span><span class="sxs-lookup"><span data-stu-id="bf3a3-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="bf3a3-104">In der Regel dauert es nur ein paar Minuten, bis wir den neuen Eintrag sehen können, aber gelegentlich kann es auch ein paar Stunden dauern.</span><span class="sxs-lookup"><span data-stu-id="bf3a3-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="bf3a3-105">Wenn Sie schon lange gewartet haben, überprüfen Sie, ob Sie den genauen Wert kopiert und in den TXT-Überprüfungs Eintrag bei Ihrem DNS-Host eingefügt haben.</span><span class="sxs-lookup"><span data-stu-id="bf3a3-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="bf3a3-106">Ein häufiges Problem ist, dass der Teil "MS=" des Eintrags fehlt.</span><span class="sxs-lookup"><span data-stu-id="bf3a3-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="bf3a3-107">Diese Angabe ist ebenfalls erforderlich!</span><span class="sxs-lookup"><span data-stu-id="bf3a3-107">We need that too!</span></span>
    
- <span data-ttu-id="bf3a3-108">Bei einigen DNS-Hosts müssen Sie einen zusätzlichen Schritt ausführen, um die Zonendatei zu speichern (in der der DNS-Eintrag gespeichert ist), damit der Eintrag im Internet aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="bf3a3-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="bf3a3-109">Stellen Sie sicher, dass Sie die Änderungen gespeichert haben, damit der Eintrag von Office 365 angezeigt und überprüft werden kann.</span><span class="sxs-lookup"><span data-stu-id="bf3a3-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

