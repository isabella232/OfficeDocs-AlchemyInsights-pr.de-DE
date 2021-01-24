---
title: SCIM-Bereitstellungsprobleme
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935378"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="0a0b6-102">SCIM-Bereitstellungsprobleme</span><span class="sxs-lookup"><span data-stu-id="0a0b6-102">SCIM provisioning issue</span></span>

<span data-ttu-id="0a0b6-103">Bei der automatischen Bereitstellung werden Benutzeridentitäten und Rollen in Cloud-Anwendungen erstellt, auf die Benutzer Zugriff erhalten müssen.</span><span class="sxs-lookup"><span data-stu-id="0a0b6-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="0a0b6-104">Zusätzlich zu der Erstellung von Benutzeridentitäten schließt die automatische Bereitstellung auch die Wartung und Entfernung von Benutzeridentitäten ein, wenn sich deren Status oder Rolle ändert.</span><span class="sxs-lookup"><span data-stu-id="0a0b6-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="0a0b6-105">Vor der Bereitstellung können Sie sich [So funktioniert die Bereitstellung](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) durchlesen, um zu erfahren, wie die Bereitstellung in Azure Active Directory (AD) funktioniert, und um Empfehlungen für die Konfiguration zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="0a0b6-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="0a0b6-106">Als Anwendungsentwickler können Sie die System for Cross-Domain Identity Management (SCIM)-API für die Benutzerverwaltung verwenden, um die automatische Bereitstellung von Benutzern und Gruppen zwischen Ihrer Anwendung und Azure AD zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="0a0b6-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="0a0b6-107">In dem Artikel [Erstellen eines SCIM-Endpunkts und Konfigurieren der Benutzerbereitstellung mit Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) wird beschrieben, wie ein SCIM-Endpunkt erstellt und mit dem Bereitstellungsdienst in Azure Ad integriert wird.</span><span class="sxs-lookup"><span data-stu-id="0a0b6-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



