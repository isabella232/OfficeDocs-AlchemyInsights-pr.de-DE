---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821446"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="efa87-102">Beheben von Übermittlungsproblemen für Fehlercode 550 5.4.1 Relayzugriff verweigert</span><span class="sxs-lookup"><span data-stu-id="efa87-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="efa87-103">Dieses Problem tritt auf, wenn überprüft wird, ob eine E-Mail-Adresse gültig ist, um [Bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) beim Betreten des Microsoft-Netzwerks zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="efa87-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="efa87-104">Versuchen Sie, das Problem durch folgende Maßnahme zu beheben:</span><span class="sxs-lookup"><span data-stu-id="efa87-104">Try the following:</span></span>

1. <span data-ttu-id="efa87-105">Ermitteln Sie, ob das Problem für eine gesamte Domäne oder eine einzelne E-Mail-Adresse spezifisch ist:</span><span class="sxs-lookup"><span data-stu-id="efa87-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="efa87-106">Gesamte Domäne: Manchmal muss die Domäne synchronisiert werden. versuchen [Sie, die Domäne auf Internal und dann zurück auf Autoritative zu setzen.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="efa87-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="efa87-107">Einzelne E-Mail-Adresse: Manchmal muss die Adresse synchronisiert werden. Das Ändern der SMTP-Proxyadresse und das anschließende Ändern der Smtpproxyadresse können hilfreich sein.</span><span class="sxs-lookup"><span data-stu-id="efa87-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="efa87-108">Ermitteln Sie, ob das Problem für eine Gruppe oder einen öffentlichen Ordner spezifisch ist.</span><span class="sxs-lookup"><span data-stu-id="efa87-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="efa87-109">Bei einigen Objekttypen müssen die Objekte möglicherweise manuell in Azure Active Directory erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="efa87-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="efa87-110">Wenn Sie zusätzliche Hilfe benötigen, öffnen Sie bitte ein Supportticket, und geben Sie den Umfang des Problems an (einschließlich des Typs des Objekts, an das Sie senden), damit wir Sie besser unterstützen können.</span><span class="sxs-lookup"><span data-stu-id="efa87-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>