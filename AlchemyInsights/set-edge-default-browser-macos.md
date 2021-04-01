---
title: Microsoft Edge als Standardbrowser auf einem MacOS-Gerät festlegen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426819"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="7cacd-102">Microsoft Edge als Standardbrowser auf einem MacOS-Gerät festlegen</span><span class="sxs-lookup"><span data-stu-id="7cacd-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="7cacd-103">Verwenden Sie eine dieser beiden Methoden, um Microsoft Edge als Standardbrowser festzulegen:</span><span class="sxs-lookup"><span data-stu-id="7cacd-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="7cacd-104">Methode 1: Blitzen Sie das Gerät mit einem Bild von MacOS, in dem Microsoft Edge bereits als Standardbrowser festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="7cacd-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="7cacd-105">Methode 2: Legen Sie die Richtlinie DefaultBrowserSettingEnabled so fest, dass der Benutzer aufgefordert wird, Microsoft Edge als Standardbrowser festzulegen.</span><span class="sxs-lookup"><span data-stu-id="7cacd-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="7cacd-106">Bei beiden Methoden kann ein Benutzer den Standardbrowser ändern.</span><span class="sxs-lookup"><span data-stu-id="7cacd-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="7cacd-107">Aus diesem Grund empfehlen wir, die Richtlinie DefaultBrowserSettingEnabled auch dann einzusetzen, wenn Sie Methode 1 verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="7cacd-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="7cacd-108">Wenn ein Benutzer den Standardbrowser ändert, nachdem die Richtlinie bereitgestellt wurde, fordert die Richtlinie den Benutzer auf, den Standardbrowser wieder auf Microsoft Edge zu setzen.</span><span class="sxs-lookup"><span data-stu-id="7cacd-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
