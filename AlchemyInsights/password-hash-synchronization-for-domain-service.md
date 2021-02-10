---
title: Kennworthashsynchronisierung für Domänendienst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162922"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="7d0ff-102">Kennworthashsynchronisierung für Domänendienst</span><span class="sxs-lookup"><span data-stu-id="7d0ff-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="7d0ff-103">**Wenn Sie von Ihrer Azure AD DS-Instanz aufgefordert werden, die Kennworthashsynchronisierung zu aktivieren**</span><span class="sxs-lookup"><span data-stu-id="7d0ff-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="7d0ff-104">Es trifft ein Szenario ein, in dem eine Hybridumgebung mit Benutzern ausgeführt wird, die aus einer lokalen Azure Active Directory Domain Services-Umgebung (AD DS) synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="7d0ff-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="7d0ff-105">Dieses Szenario ist eingetreten, obwohl die Kennworthashsynchronisierung zwischen dem lokalen AD DS und Ihrem Azure AD-Mandanten besteht.</span><span class="sxs-lookup"><span data-stu-id="7d0ff-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="7d0ff-106">**Ursache**</span><span class="sxs-lookup"><span data-stu-id="7d0ff-106">**Cause**</span></span>

<span data-ttu-id="7d0ff-107">Dies geschieht, weil Azure AD Connect standardmäßig keine älteren New Technology LAN Manager (NTLM)- und Kerberos-Kennworthashwerte synchronisiert, die für Azure AD DS erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7d0ff-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="7d0ff-108">**Problemumgehung**</span><span class="sxs-lookup"><span data-stu-id="7d0ff-108">**Workaround**</span></span> 

<span data-ttu-id="7d0ff-109">Sie müssen Azure AD Connect so konfigurieren, dass diese Kennworthashwerte synchronisiert werden, die für die NTLM- und Kerberos-Authentifizierung erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7d0ff-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="7d0ff-110">Nachdem Azure AD Connect konfiguriert wurde, werden bei der Erstellung eines lokalen Kontos oder einem Kennwortänderungsereignis auch ältere Kennworthashwerte mit Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="7d0ff-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="7d0ff-111">Weitere Informationen hierzu und Anleitungen zum Aktivieren der Kennwortsynchronisierung in Azure AD DS-Hybridumgebungen finden Sie [hier](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).</span><span class="sxs-lookup"><span data-stu-id="7d0ff-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>