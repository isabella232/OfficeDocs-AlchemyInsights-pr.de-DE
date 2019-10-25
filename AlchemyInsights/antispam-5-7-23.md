---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682136"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="5a98d-102">Beheben von Problemen mit der Zustellung von e-Mails bei Fehlercode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="5a98d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="5a98d-103">Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einem öffentlich verfügbaren SPF-oder DNS-Eintrags Prüfer im Internet.</span><span class="sxs-lookup"><span data-stu-id="5a98d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="5a98d-104">Stellen Sie sicher, dass die ausgehende Nachricht von Office 365 nicht als Spam identifiziert und über den [Pool mit hoher Risikoverteilung](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)weitergeleitet wurde.</span><span class="sxs-lookup"><span data-stu-id="5a98d-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="5a98d-105">Nachrichten im Pool mit hoher Risikoverteilung werden keine SPF-Prüfungen übergeben und werden daher von der Ziel-e-Mail-Organisation nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="5a98d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="5a98d-106">Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des e-Mail-Hosts wenden, an den Sie e-Mails senden möchten.</span><span class="sxs-lookup"><span data-stu-id="5a98d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="5a98d-107">Notieren Sie sich den detaillierten externen Fehler, der in der Bounce-Nachricht verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="5a98d-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="5a98d-108">Office 365 Support kann möglicherweise nicht weiterhelfen.</span><span class="sxs-lookup"><span data-stu-id="5a98d-108">Office 365 support may not be able to assist further.</span></span>