---
title: Virtuelle Konfiguration mit AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884581"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="7d71e-102">Virtuelle Konfiguration mit AAD Domain Services</span><span class="sxs-lookup"><span data-stu-id="7d71e-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="7d71e-103">Die virtuelle Konfiguration mit AAD Domain Services umfasst die folgenden Schritte:</span><span class="sxs-lookup"><span data-stu-id="7d71e-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="7d71e-104">Überprüfen des Integritätszustands Ihrer Domäne im Azure-Portal https://aka.ms/aadds-health.</span><span class="sxs-lookup"><span data-stu-id="7d71e-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="7d71e-105">Überprüfen Ihres NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in den Azure AD Domain Services im Portal https://aka.ms/aadds-networking erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7d71e-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="7d71e-106">Sicherstellen, dass Ihr virtuelles Netzwerk in derselben Azure-Region wie die von Azure AD Domain Services verwaltete Domäne bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="7d71e-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="7d71e-107">Sicherstellen, dass Sie nicht über eine vorhandene Domäne mit demselben Domänennamen verfügen, die im virtuellen Netzwerk verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="7d71e-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="7d71e-108">Weitere Details zu Designüberlegungen zum virtuellen Netzwerk von Azure zur Unterstützung von AAD Domain Services finden Sie unter [Überlegungen zum virtuellen Netzwerk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="7d71e-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

