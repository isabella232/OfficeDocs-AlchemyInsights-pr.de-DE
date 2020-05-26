---
title: Beheben von Problemen mit der SMTP-Authentifizierung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264429"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="3cc5f-102">Beheben von Problemen mit der SMTP-Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="3cc5f-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="3cc5f-103">Wenn Sie beim Versuch, eine SMTP-E-Mail zu versenden und diese über einen Client oder eine Anwendung zu authentifizieren, die Fehlermeldungen 5.7.57 oder 5.7.3 erhalten, sollten Sie Folgendes überprüfen:</span><span class="sxs-lookup"><span data-stu-id="3cc5f-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="3cc5f-104">Die authentifizierte SMTP-Übermittlung ist möglicherweise in Ihrem Mandanten oder dem Postfach, das Sie verwenden möchten, deaktiviert (überprüfen Sie beide Einstellungen).</span><span class="sxs-lookup"><span data-stu-id="3cc5f-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="3cc5f-105">Weitere Informationen finden Sie unter [Authentifizierte Client-SMTP-Übermittlung aktivieren oder deaktivieren](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="3cc5f-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="3cc5f-106">Überprüfen Sie, ob [Azure Sicherheitsvorgaben](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) für Ihren Mandanten aktiviert sind. Wenn diese Option aktiviert ist, schlägt die SMTP-Authentifizierung mithilfe der Standardauthentifizierung (auch als „Legacy-Authentifizierung“ bekannt; diese verwendet Benutzernamen und Kennwort) fehl.</span><span class="sxs-lookup"><span data-stu-id="3cc5f-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
