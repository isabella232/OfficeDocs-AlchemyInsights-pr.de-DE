---
title: Antispam 5.4.1 Blockierung catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707910"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="9aec3-102">Beheben von Übermittlungsproblemen für den Fehlercode 550 5.4.1 Relay-Zugriff verweigert</span><span class="sxs-lookup"><span data-stu-id="9aec3-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="9aec3-103">Dieses Problem tritt auf [, wenn Sie überprüfen, ob eine e-Mail-Adresse gültig ist, um Abpraller](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) beim Eindringen in das Microsoft-Netzwerk zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="9aec3-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="9aec3-104">Versuchen Sie, das Problem durch folgende Maßnahme zu beheben:</span><span class="sxs-lookup"><span data-stu-id="9aec3-104">Try the following:</span></span>

1. <span data-ttu-id="9aec3-105">Ermitteln, ob das Problem für eine ganze Domäne oder eine einzelne e-Mail-Adresse spezifisch ist:</span><span class="sxs-lookup"><span data-stu-id="9aec3-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="9aec3-106">Gesamte Domäne: Manchmal muss die Domäne synchronisiert werden; versuchen Sie [, die Domäne auf Internal und dann auf autorisierend zurücksetzen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="9aec3-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="9aec3-107">Einzelne e-Mail-Adresse: Manchmal muss die Adresse synchronisiert werden; Wenn Sie die SMTP-Proxyadresse ändern und dann zurück ändern, kann dies hilfreich sein.</span><span class="sxs-lookup"><span data-stu-id="9aec3-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="9aec3-108">Ermitteln Sie, ob das Problem für eine Gruppe oder einen öffentlichen ordnerspezifisch ist.</span><span class="sxs-lookup"><span data-stu-id="9aec3-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="9aec3-109">Für einige Objekttypen müssen die Objekte möglicherweise manuell in Azure Active Directory erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9aec3-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="9aec3-110">Wenn Sie weitere Hilfe benötigen, öffnen Sie ein Support Ticket, und geben Sie den Umfang des Problems an (einschließlich des Typs des Objekts, an das Sie senden), damit wir Sie besser unterstützen können.</span><span class="sxs-lookup"><span data-stu-id="9aec3-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>