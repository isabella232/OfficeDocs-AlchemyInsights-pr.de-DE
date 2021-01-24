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
# <a name="user-provisioning-attribute-mapping"></a>Attributzuordnung für die Benutzerbereitstellung

1. Hinweise zur Behandlung bekannter Probleme mit der Attributzuordnung finden Sie unter [Attributzuordnungen](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) bietet Unterstützung bei der Benutzerbereitstellung auf SaaS-Anwendungen von Drittanbietern wie Salesforce, G Suite und weitere. Wenn Sie die Benutzerbereitstellung für eine SaaS-Anwendung von Drittanbietern aktivieren, steuert das Azure-Portal die Attributwerte durch Attributzuordnungen. Unter [Anpassen von Attributzuordnungen bei der Benutzerbereitstellung für SaaS-Anwendungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes) erfahren Sie, wie Sie die standardmäßigen Attributzuordnungen anpassen können.
    - Mehr über die Benutzerbereitstellung in SaaS-Anwendungen lernen Sie unter [Was ist die automatische Benutzerbereitstellung in SaaS-Anwendungen in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Bei der Anpassung von Attributzuordnungen für die Benutzerbereitstellung merken Sie unter Umständen, dass das Attribut, das Sie zuordnen möchten, nicht in der Liste mit Quellattributen erscheint. Der Artikel [Synchronisieren eines Attributs von Ihrem Windows Server AD auf Azure AD für die Bereitstellung in einer Anwendung](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) zeigt Ihnen, wie Sie das fehlende Attribut hinzufügen, indem Sie es von Ihrem Windows Server AD auf Azure AD synchronisieren.
