---
title: Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827516"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="4d99b-102">Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen</span><span class="sxs-lookup"><span data-stu-id="4d99b-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="4d99b-103">Wechseln Sie im Microsoft 365 Admin Center zur Seite Setupdomänen, und wählen Sie in der Liste der Domänen die Domäne aus, die Sie für  >  [](https://admin.microsoft.com/Adminportal#/Domains) Ihre Website verwenden.</span><span class="sxs-lookup"><span data-stu-id="4d99b-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="4d99b-104">Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="4d99b-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4d99b-105">Geben Sie unter **DNS-Typ** ein: **A (Adresse)**</span><span class="sxs-lookup"><span data-stu-id="4d99b-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="4d99b-106">Geben Sie unter **Hostname oder Alias** Folgendes ein: **@**</span><span class="sxs-lookup"><span data-stu-id="4d99b-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="4d99b-107">Geben Sie unter **IP-Adresse** die statische IP-Adresse für Ihre Website ein, unter der diese derzeit gehostet wird, beispielsweise "172.16.140.1".</span><span class="sxs-lookup"><span data-stu-id="4d99b-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="4d99b-p101">Es muss eine  *statische*  IP-Adresse für die Website sein, keine  *dynamische*  . Überprüfen Sie bei der Website, auf der Ihre Website gehostet wird, dass Sie eine statische IP-Adresse für Ihre öffentliche Website erhalten können.</span><span class="sxs-lookup"><span data-stu-id="4d99b-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="4d99b-110">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="4d99b-110">Select **Save**.</span></span>

<span data-ttu-id="4d99b-111">Darüber hinaus können Sie einen CNAME-Eintrag erstellen, damit Kunden Ihre Website besser finden können.</span><span class="sxs-lookup"><span data-stu-id="4d99b-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="4d99b-112">Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="4d99b-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4d99b-113">Geben Sie unter **DNS-Typ** ein: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="4d99b-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="4d99b-114">Geben Sie unter **Hostname oder Alias** Folgendes ein: **www**</span><span class="sxs-lookup"><span data-stu-id="4d99b-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="4d99b-115">Geben Sie unter **Verweist auf die Adresse** den vollqualifizierten Domänennamen (Fully Qualified Domain Name, FQDN) Ihrer Website ein, beispielsweise contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4d99b-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="4d99b-116">Wählen Sie **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="4d99b-116">Select **Save**.</span></span>
