---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820177"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="22365-102">Blockieren der Legacyauthentifizierung</span><span class="sxs-lookup"><span data-stu-id="22365-102">Blocking legacy authentication</span></span>

<span data-ttu-id="22365-103">Der Begriff Legacy-Authentifizierung bezeichnet eine Authentifizierungsanforderung folgender Clients:</span><span class="sxs-lookup"><span data-stu-id="22365-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="22365-104">Ältere Office-Clients, die keine moderne Authentifizierung verwenden (z. B. Office 2010-Client).</span><span class="sxs-lookup"><span data-stu-id="22365-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="22365-105">Alle Clients, die Legacy-Mail-Protokolle wie IMAP/SMTP/POP3 verwenden.</span><span class="sxs-lookup"><span data-stu-id="22365-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="22365-106">Weitere Informationen zum Blockieren der Legacyauthentifizierung und zum Aktivieren der modernen Authentifizierung finden Sie unter [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="22365-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="22365-107">Sicherheitseinstellungen in Azure Active Directory (Azure AD) erleichtern die Sicherheit und schützen Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="22365-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="22365-108">Sicherheitseinstellungen enthalten vorkonfigurierte Sicherheitseinstellungen für häufige Angriffe.</span><span class="sxs-lookup"><span data-stu-id="22365-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="22365-109">Weitere Informationen zu Sicherheitseinstellungen finden Sie unter [Was sind Sicherheitseinstellungen?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="22365-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="22365-110">**Hinweis**: Wenn Ihr Mandant am oder nach dem 22. Oktober 2019 erstellt wurde, ist es möglich, dass Sie das neue standardmäßige Sicherheitsverhalten erleben und bereits Sicherheitseinstellungen in Ihrem Mandanten aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="22365-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="22365-111">Um alle Benutzer zu schützen, werden Sicherheitseinstellungen für alle neuen Mandanten erstellt.</span><span class="sxs-lookup"><span data-stu-id="22365-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
