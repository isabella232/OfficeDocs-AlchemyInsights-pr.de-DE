---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685597"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="6cea8-102">Blockieren der Legacy Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="6cea8-102">Blocking legacy authentication</span></span>

<span data-ttu-id="6cea8-103">Der Begriff Legacy-Authentifizierung bezeichnet eine Authentifizierungsanforderung folgender Clients:</span><span class="sxs-lookup"><span data-stu-id="6cea8-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="6cea8-104">Ältere Office-Clients, die keine moderne Authentifizierung verwenden (beispielsweise Office 2010-Client).</span><span class="sxs-lookup"><span data-stu-id="6cea8-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="6cea8-105">Alle Clients, die Legacy-Mail-Protokolle wie IMAP/SMTP/POP3 verwenden.</span><span class="sxs-lookup"><span data-stu-id="6cea8-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="6cea8-106">Weitere Informationen zum Blockieren der Legacy Authentifizierung und zur Aktivierung moderner Authentifizierung finden Sie unter [Blockieren der Legacy](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="6cea8-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="6cea8-107">Sicherheitsstandards in Azure Active Directory (Azure AD) erleichtern die Sicherheit und schützen Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="6cea8-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="6cea8-108">Sicherheitsstandards enthalten vorkonfigurierte Sicherheitseinstellungen für häufige Angriffe.</span><span class="sxs-lookup"><span data-stu-id="6cea8-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="6cea8-109">Weitere Informationen zu Sicherheitsstandards finden Sie unter [Was sind Sicherheitsstandards?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="6cea8-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="6cea8-110">**Hinweis**: Wenn Ihr Mandant am oder nach dem 22. Oktober 2019 erstellt wurde, ist es möglich, dass Sie das neue Standardverhalten durchlaufen und bereits Sicherheitsstandards in Ihrem Mandanten aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="6cea8-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="6cea8-111">In dem Bemühen, alle unsere Benutzer zu schützen, werden Sicherheitsstandards für alle neuen erstellten Mandanten eingeführt.</span><span class="sxs-lookup"><span data-stu-id="6cea8-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
