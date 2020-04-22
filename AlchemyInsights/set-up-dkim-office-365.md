---
title: Setup-DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645671"
---
# <a name="setup-dkim"></a><span data-ttu-id="c7f47-102">Setup-DKIM</span><span class="sxs-lookup"><span data-stu-id="c7f47-102">Setup DKIM</span></span>

<span data-ttu-id="c7f47-103">Die vollständigen Anweisungen zum Konfigurieren von DKIM für benutzerdefinierte Domänen in Microsoft 365 finden Sie [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="c7f47-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="c7f47-104">Für **jede** benutzerdefinierte Domäne müssen Sie **zwei** DKIM-CNAME-Einträge im DNS-Hostingdienst Ihrer Domäne erstellen (in der Regel die Domänenregistrierungsstelle).</span><span class="sxs-lookup"><span data-stu-id="c7f47-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="c7f47-105">Für contoso.com und fourthcoffee.com sind beispielsweise vier DKIM-CNAME-Einträge erforderlich: zwei für contoso.com und zwei für fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="c7f47-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="c7f47-106">Die DKIM-CNAME-Einträge für **jede** benutzerdefinierte Domäne verwenden die folgenden Formate:</span><span class="sxs-lookup"><span data-stu-id="c7f47-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="c7f47-107">**Hostname**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="c7f47-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="c7f47-108">**Verweist auf Adresse oder Wert**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="c7f47-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="c7f47-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="c7f47-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="c7f47-110">**Hostname**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="c7f47-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="c7f47-111">**Verweist auf Adresse oder Wert**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="c7f47-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="c7f47-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="c7f47-112">**TTL**: 3600</span></span>

   <span data-ttu-id="c7f47-113">\<DomainGUID\> ist der Text Links `.mail.protection.outlook.com` neben dem angepassten MX-Eintrag für die benutzerdefinierte Domäne (beispielsweise `contoso-com` für die Domäne contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c7f47-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="c7f47-114">\<InitialDomain\> ist die Domäne, die Sie bei der Registrierung bei Microsoft 365 verwendet haben (beispielsweise contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="c7f47-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="c7f47-115">Nachdem Sie die CNAME-Einträge für Ihre benutzerdefinierten Domänen erstellt haben, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="c7f47-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="c7f47-116">a.</span><span class="sxs-lookup"><span data-stu-id="c7f47-116">a.</span></span> <span data-ttu-id="c7f47-117">[melden Sie sich bei Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) mit ihrem geschäftlichen oder Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="c7f47-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="c7f47-118">b.</span><span class="sxs-lookup"><span data-stu-id="c7f47-118">b.</span></span> <span data-ttu-id="c7f47-119">Klicken Sie oben links auf das App-Startsymbol, und wählen Sie **Admin** aus.</span><span class="sxs-lookup"><span data-stu-id="c7f47-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="c7f47-120">c.</span><span class="sxs-lookup"><span data-stu-id="c7f47-120">c.</span></span> <span data-ttu-id="c7f47-121">Erweitern Sie im unteren linken Navigationsbereich **Admin**, und klicken Sie dann auf **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c7f47-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="c7f47-122">d.</span><span class="sxs-lookup"><span data-stu-id="c7f47-122">d.</span></span> <span data-ttu-id="c7f47-123">Wechseln Sie zu **Protection** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="c7f47-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="c7f47-124">e.</span><span class="sxs-lookup"><span data-stu-id="c7f47-124">e.</span></span> <span data-ttu-id="c7f47-125">Wählen Sie die Domäne aus, und wählen Sie dann für **Signieren Nachrichten für diese Domäne mit DKIM-Signaturen** **aktivieren** aus.</span><span class="sxs-lookup"><span data-stu-id="c7f47-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="c7f47-126">Wiederholen Sie diesen Schritt für jede benutzerdefinierte Domäne.</span><span class="sxs-lookup"><span data-stu-id="c7f47-126">Repeat this step for each custom domain.</span></span>
