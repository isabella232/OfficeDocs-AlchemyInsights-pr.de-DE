---
title: Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552438"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="cc619-102">Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)</span><span class="sxs-lookup"><span data-stu-id="cc619-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="cc619-103">Eine Antispamrichtlinie in Ihrem Mandanten hat diese Nachricht beeinflusst.</span><span class="sxs-lookup"><span data-stu-id="cc619-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="cc619-104">Gehen Sie wie folgt vor, um die Richtlinie zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="cc619-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="cc619-105">Wechseln Sie zum [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)und wechseln Sie dann zu **Bedrohungsverwaltungsrichtlinie**  >    >  [Antispam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="cc619-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="cc619-106">Überprüfen Sie, ob **die Richtlinienquelle** Folgendes angibt:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="cc619-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="cc619-107">Wenn ja, überprüfen **Sie** auf der Registerkarte Benutzerdefinierte Die Einstellungen der Richtlinie, die sich auf die Nachricht ausdingt.</span><span class="sxs-lookup"><span data-stu-id="cc619-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="cc619-108">Es ist möglich, dass die **Standardeinstellungen, die** auf alle Exchange Online Protection-Kunden angewendet wurden, die Nachricht beeinflusst haben.</span><span class="sxs-lookup"><span data-stu-id="cc619-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="cc619-109">Weitere Informationen zum Konfigurieren von Spamfilterrichtlinien finden Sie unter [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="cc619-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
