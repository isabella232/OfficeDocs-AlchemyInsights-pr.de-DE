---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717324"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="84f2e-102">Beheben von Problemen mit der Zustellung von e-Mails bei Fehlercode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="84f2e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="84f2e-103">Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einem öffentlich verfügbaren SPF-oder DNS-Eintrags Prüfer im Internet.</span><span class="sxs-lookup"><span data-stu-id="84f2e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="84f2e-104">Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den [Pool mit hoher Risikoverteilung](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)weitergeleitet wurde.</span><span class="sxs-lookup"><span data-stu-id="84f2e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="84f2e-105">Nachrichten im Pool mit hoher Risikoverteilung werden keine SPF-Prüfungen übergeben und werden daher von der Ziel-e-Mail-Organisation nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="84f2e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="84f2e-106">Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des e-Mail-Hosts wenden, an den Sie e-Mails senden möchten.</span><span class="sxs-lookup"><span data-stu-id="84f2e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="84f2e-107">Notieren Sie sich den detaillierten externen Fehler, der in der Bounce-Nachricht verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="84f2e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="84f2e-108">Der Microsoft-Support kann möglicherweise nicht weiterhelfen.</span><span class="sxs-lookup"><span data-stu-id="84f2e-108">Microsoft support may not be able to assist further.</span></span>
