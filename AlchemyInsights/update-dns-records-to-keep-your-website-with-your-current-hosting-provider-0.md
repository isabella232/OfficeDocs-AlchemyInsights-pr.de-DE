---
title: Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469986"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="837fc-102">Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen</span><span class="sxs-lookup"><span data-stu-id="837fc-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="837fc-103">Wählen Sie auf der Seite [Domänen](https://portal.office.com/adminportal/home#/Domains) in der Liste der Domänen die Domäne aus, die Sie für Ihre Website verwenden, und wählen Sie dann im Verwaltungsbereich **DNS-Einstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="837fc-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="837fc-104">Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="837fc-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="837fc-105">Geben Sie unter **DNS-Typ** ein: **A (Adresse)**</span><span class="sxs-lookup"><span data-stu-id="837fc-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="837fc-106">Geben Sie unter **Hostname oder Alias** Folgendes ein: **@**</span><span class="sxs-lookup"><span data-stu-id="837fc-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="837fc-107">Geben Sie unter **IP-Adresse** die statische IP-Adresse für Ihre Website ein, unter der diese derzeit gehostet wird, beispielsweise "172.16.140.1".</span><span class="sxs-lookup"><span data-stu-id="837fc-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="837fc-p101">Es muss eine  *statische*  IP-Adresse für die Website sein, keine  *dynamische*  . Überprüfen Sie bei der Website, auf der Ihre Website gehostet wird, dass Sie eine statische IP-Adresse für Ihre öffentliche Website erhalten können.</span><span class="sxs-lookup"><span data-stu-id="837fc-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="837fc-110">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="837fc-110">Select **Save**.</span></span> 
    
<span data-ttu-id="837fc-111">Darüber hinaus können Sie einen CNAME-Eintrag erstellen, damit Kunden Ihre Website besser finden können.</span><span class="sxs-lookup"><span data-stu-id="837fc-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="837fc-112">Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="837fc-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="837fc-113">Geben Sie unter **DNS-Typ** ein: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="837fc-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="837fc-114">Geben Sie unter **Hostname oder Alias** Folgendes ein: **www**</span><span class="sxs-lookup"><span data-stu-id="837fc-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="837fc-115">Geben Sie unter **Verweist auf die Adresse** den vollqualifizierten Domänennamen (Fully Qualified Domain Name, FQDN) Ihrer Website ein, beispielsweise contoso.com.</span><span class="sxs-lookup"><span data-stu-id="837fc-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="837fc-116">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="837fc-116">Select **Save**.</span></span> 
    

