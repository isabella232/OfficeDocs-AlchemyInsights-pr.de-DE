---
title: Anhalten geplanter Updates
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721554"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="033f3-102">Anhalten geplanter Updates</span><span class="sxs-lookup"><span data-stu-id="033f3-102">Pausing scheduled updates</span></span>

<span data-ttu-id="033f3-103">Wenn ein Pausenbefehl ausgegeben wird, verarbeiten die Geräte den Befehl erst beim nächsten Einchecken bei Intune.</span><span class="sxs-lookup"><span data-stu-id="033f3-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="033f3-104">Aus diesem Grund wurden für Ihre Geräte möglicherweise folgende Aktionen aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="033f3-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="033f3-105">Die geplanten Updates wurden bereits vor dem Einchecken installiert.</span><span class="sxs-lookup"><span data-stu-id="033f3-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="033f3-106">Das Gerät wurde ausgeschaltet, als Sie den Befehl "Anhalten" ausgegeben haben.</span><span class="sxs-lookup"><span data-stu-id="033f3-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="033f3-107">In diesem Fall wurden die geplanten Updates möglicherweise vor dem Einchecken heruntergeladen und installiert, wenn die Geräte eingeschaltet waren.</span><span class="sxs-lookup"><span data-stu-id="033f3-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>