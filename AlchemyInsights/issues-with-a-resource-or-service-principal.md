---
title: Probleme mit einem Ressourcen- oder Dienstprinzipal
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716126"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Probleme mit einem Ressourcen- oder Dienstprinzipal

1. Wenn Sie gerade erst beginnen, beschreiben Anwendungs- und Dienstprinzipalobjekte [in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) die Anwendungsregistrierung, Anwendungsobjekte und Dienstprinzipale in Azure Active Directory: was sie sind, wie sie verwendet werden und wie sie miteinander in Beziehung stehen. Ein Beispielszenario mit mehreren Mandanten wird ebenfalls dargestellt, um die Beziehung zwischen dem Anwendungsobjekt einer Anwendung und den entsprechenden Dienstprinzipalobjekten zu veranschaulichen.
2. Weitere Informationen zur Beziehung zwischen Anwendungen und Dienstprinzipalnamen finden Sie unter Lesen von [Anwendungen und Dienstprinzipalobjekten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [How to:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Use the portal to create an Azure AD application and service principal that can access resources shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Mit der [Dienstprinzipal-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)können Sie Anwendungsinstanzen programmgesteuert verwalten und steuern, was eine Anwendung innerhalb Ihres Mandanten tun kann.
5. [der servicePrincipal-Ressourcentyp](https://docs.microsoft.com/graph/api/resources/serviceprincipal) listet alle Eigenschaften und Methoden für den servicePrincipal-Ressourcentyp auf.
6. [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph stellen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) Unterschiede zwischen Azure AD Graph und Microsoft Graph-Ressourcen dar. Es zeigt Ressourcen an, die unterschiedliche Namen haben oder nicht verfügbar sind. Außerdem werden Ressourcen hervorgehoben, die in der Betaversion von Microsoft Graph, aber nicht in der Version v1.0 verfügbar sind.

**Probleme mit Gastbenutzern**

- [Schnellstart:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Hinzufügen von Gastbenutzern zu Ihrem Verzeichnis im Azure-Portal zeigt Ihnen, wie Sie ihrem Azure AD-Verzeichnis über das Azure-Portal einen neuen Gastbenutzer hinzufügen, eine Einladung senden und sehen, wie der Einladungseinlösungsprozess des Gastbenutzers aussieht.
- [Lernprogramm: Erstellen von Benutzerflüssen in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) zeigt, wie Sie einige empfohlene Benutzerflüsse mithilfe des Azure-Portals erstellen. Wenn Sie Informationen zum Einrichten eines RoPC (Resource Owner Password Credentials) in Ihrer Anwendung suchen, finden Sie weitere Informationen unter Configure the resource owner password credentials flow in Azure AD B2C.
