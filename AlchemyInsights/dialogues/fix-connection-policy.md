---
title: Fix connection policy
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568565"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="bcd32-102">Fix connection policy</span><span class="sxs-lookup"><span data-stu-id="bcd32-102">Fix connection policy</span></span>

<span data-ttu-id="bcd32-103">Die E-Mail wurde als sicher gekennzeichnet und an den Posteingang des Benutzers übermittelt, da die sendende IP-Adresse in der Verbindungsfilterrichtlinie als sicher gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="bcd32-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="bcd32-104">Gehen Sie wie folgt vor, um die Richtlinie zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="bcd32-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="bcd32-105">Wechseln Sie zum [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)und wechseln Sie dann zu **Bedrohungsverwaltungsrichtlinie**  >    >  [Antispam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="bcd32-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="bcd32-106">Wählen Sie **auf** der Registerkarte Benutzerdefinierte Die **Verbindungsfilterrichtlinie** aus, und wählen Sie dann **Richtlinie bearbeiten aus.**</span><span class="sxs-lookup"><span data-stu-id="bcd32-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="bcd32-107">Überprüfen Sie die **Liste der zulässigen IP-Adressen.**</span><span class="sxs-lookup"><span data-stu-id="bcd32-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="bcd32-108">Sehen Sie, **ob die Liste "Sicher"** aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="bcd32-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="bcd32-109">Microsoft hat verschiedene Quellen von Drittanbietern mit vertrauenswürdigen Absendern abonniert.</span><span class="sxs-lookup"><span data-stu-id="bcd32-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="bcd32-110">Wenn **die Liste "Sicher"** aktiviert ist, werden diese vertrauenswürdigen Absender nicht fälschlicherweise als Spam gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="bcd32-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="bcd32-111">Ich empfehle, diese Option zu wählen, da dadurch die Anzahl falsch positiver Nachrichten (gute E-Mails, die als Spam klassifiziert werden) reduziert wird, die Sie erhalten.</span><span class="sxs-lookup"><span data-stu-id="bcd32-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
