---
title: Für die Wiedergabe von Videos verwendetes CDN
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: d9c5f8f586e7f5aa079b28584375516ec8401ca7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819367"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="77755-102">Für die Wiedergabe von Videos verwendetes CDN</span><span class="sxs-lookup"><span data-stu-id="77755-102">CDN used for video playback</span></span>

<span data-ttu-id="77755-103">Liveereignisse aus Stream sowie Liveereignisse externer Apps oder Geräte aus Yammer/Teams verwenden automatisch Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="77755-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="77755-104">Bei Bedarf in Stream hochgeladene Videos verwenden Azure CDN noch nicht zur Wiedergabe.</span><span class="sxs-lookup"><span data-stu-id="77755-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="77755-105">Nicht-Livevideos werden über den Ursprungsserver von Azure Media Services wiedergegeben, der Ihrem Mandanten in seiner geografischen Region zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="77755-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="77755-106">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="77755-106">For more information, see:</span></span>

- [<span data-ttu-id="77755-107">Für die Wiedergabe von Videos verwendetes CDN</span><span class="sxs-lookup"><span data-stu-id="77755-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
