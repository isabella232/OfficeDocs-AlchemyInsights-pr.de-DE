---
title: Anhalten geplanter Updates
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530589"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="65eb6-102">Anhalten geplanter Updates</span><span class="sxs-lookup"><span data-stu-id="65eb6-102">Pausing scheduled updates</span></span>

<span data-ttu-id="65eb6-103">Wenn ein Pausenbefehl ausgegeben wird, verarbeiten die Geräte den Befehl erst beim nächsten Einchecken bei Intune.</span><span class="sxs-lookup"><span data-stu-id="65eb6-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="65eb6-104">Aus diesem Grund wurden für Ihre Geräte möglicherweise folgende Aktionen aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="65eb6-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="65eb6-105">Die geplanten Updates wurden bereits vor dem Einchecken installiert.</span><span class="sxs-lookup"><span data-stu-id="65eb6-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="65eb6-106">Das Gerät wurde ausgeschaltet, als Sie den Befehl "Anhalten" ausgegeben haben.</span><span class="sxs-lookup"><span data-stu-id="65eb6-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="65eb6-107">In diesem Fall wurden die geplanten Updates möglicherweise vor dem Einchecken heruntergeladen und installiert, wenn die Geräte eingeschaltet waren.</span><span class="sxs-lookup"><span data-stu-id="65eb6-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>