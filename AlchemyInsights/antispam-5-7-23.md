---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821410"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="0e909-102">Beheben von Problemen mit der E-Mail-Zustellung für Fehlercode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="0e909-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="0e909-103">Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einer öffentlich verfügbaren SPF- oder DNS-Eintragsüberprüfung im Web.</span><span class="sxs-lookup"><span data-stu-id="0e909-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="0e909-104">Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den Pool für die Zustellung mit hohem [Risiko geroutet wurde.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="0e909-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="0e909-105">Nachrichten im Pool für die Zustellung mit hohem Risiko bestehen keine SPF-Prüfungen und werden daher von der Ziel-E-Mail-Organisation nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0e909-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="0e909-106">Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des E-Mail-Hosts wenden, an den Sie versuchen, E-Mails zu senden.</span><span class="sxs-lookup"><span data-stu-id="0e909-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="0e909-107">Notieren Sie sich den detaillierten externen Fehler in der Unzustellbarkeitsnachricht.</span><span class="sxs-lookup"><span data-stu-id="0e909-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="0e909-108">Der Microsoft-Support kann möglicherweise nicht weiter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0e909-108">Microsoft support may not be able to assist further.</span></span>
