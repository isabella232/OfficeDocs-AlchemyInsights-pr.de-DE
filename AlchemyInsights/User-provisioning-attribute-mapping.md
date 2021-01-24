---
title: Attributzuordnung für die Benutzerbereitstellung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935364"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="1daea-102">Attributzuordnung für die Benutzerbereitstellung</span><span class="sxs-lookup"><span data-stu-id="1daea-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="1daea-103">Hinweise zur Behandlung bekannter Probleme mit der Attributzuordnung finden Sie unter [Attributzuordnungen](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="1daea-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="1daea-104">Microsoft Azure Active Directory (AD) bietet Unterstützung bei der Benutzerbereitstellung auf SaaS-Anwendungen von Drittanbietern wie Salesforce, G Suite und weitere.</span><span class="sxs-lookup"><span data-stu-id="1daea-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="1daea-105">Wenn Sie die Benutzerbereitstellung für eine SaaS-Anwendung von Drittanbietern aktivieren, steuert das Azure-Portal die Attributwerte durch Attributzuordnungen.</span><span class="sxs-lookup"><span data-stu-id="1daea-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="1daea-106">Unter [Anpassen von Attributzuordnungen bei der Benutzerbereitstellung für SaaS-Anwendungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes) erfahren Sie, wie Sie die standardmäßigen Attributzuordnungen anpassen können.</span><span class="sxs-lookup"><span data-stu-id="1daea-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="1daea-107">Mehr über die Benutzerbereitstellung in SaaS-Anwendungen lernen Sie unter [Was ist die automatische Benutzerbereitstellung in SaaS-Anwendungen in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="1daea-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="1daea-108">Bei der Anpassung von Attributzuordnungen für die Benutzerbereitstellung merken Sie unter Umständen, dass das Attribut, das Sie zuordnen möchten, nicht in der Liste mit Quellattributen erscheint.</span><span class="sxs-lookup"><span data-stu-id="1daea-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="1daea-109">Der Artikel [Synchronisieren eines Attributs von Ihrem Windows Server AD auf Azure AD für die Bereitstellung in einer Anwendung](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) zeigt Ihnen, wie Sie das fehlende Attribut hinzufügen, indem Sie es von Ihrem Windows Server AD auf Azure AD synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="1daea-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
