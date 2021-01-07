---
title: Meldung „Keine Abonnements gefunden“ im Security Center
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768530"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="4cdf4-102">Meldung „Keine Abonnements gefunden“ im Security Center</span><span class="sxs-lookup"><span data-stu-id="4cdf4-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="4cdf4-103">Wenn Sie beim Zugriff auf das Microsoft Defender Security Center die Meldung „Keine Abonnements gefunden“ erhalten, bedeutet dies, dass das Azure Active Directory (AAD), mit dem sich der Benutzer am Portal anmeldet, keine Microsoft Defender ATP-Lizenz hat.</span><span class="sxs-lookup"><span data-stu-id="4cdf4-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="4cdf4-104">Die Lizenzen für Windows E5 und Office E5 sind separate Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="4cdf4-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="4cdf4-105">Öffnen Sie einen Supportfall, wenn die Lizenz erworben, aber nicht für diese AAD-Instanz bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4cdf4-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="4cdf4-106">Entweder tritt</span><span class="sxs-lookup"><span data-stu-id="4cdf4-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="4cdf4-107">ein mögliches Problem bei der Lizenzbereitstellung auf.</span><span class="sxs-lookup"><span data-stu-id="4cdf4-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="4cdf4-108">Oder Sie haben die Lizenz versehentlich für ein anderes Microsoft AAD als das für die Authentifizierung beim Dienst verwendete bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="4cdf4-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>