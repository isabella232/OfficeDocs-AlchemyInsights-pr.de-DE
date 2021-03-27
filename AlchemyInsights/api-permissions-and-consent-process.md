---
title: API-Berechtigungen und Zustimmungsprozess
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379830"
---
# <a name="api-permissions-and-consent-process"></a>API-Berechtigungen und Zustimmungsprozess

Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. [Die Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) listet die Berechtigungen auf, die den einzelnen Hauptsatz von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.

**Einrichten oder Aktualisieren des Dienstprinzipals**

- [Erstellen von serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – In diesem Artikel erfahren Sie, wie Sie ein neues servicePrincipal-Objekt erstellen.
- Erstellen einer [Azure AD-App &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Dienstprinzipal im Portal – In diesem Artikel erfahren Sie, wie Sie eine neue Azure Active Directory(Azure AD)-Anwendung und einen neuen Dienstprinzipal erstellen, die mit der rollenbasierten Zugriffssteuerung verwendet werden können.
- [Apps](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) &-Dienstprinzipale in Azure AD – In diesem Artikel wird die Anwendungsregistrierung, Anwendungsobjekte und Dienstprinzipale in Azure Active Directory beschrieben: was sie sind, wie sie verwendet werden und wie sie miteinander in Beziehung stehen.

**Hinzufügen oder Aktualisieren der App-Registrierung und Bereitstellen der Administrator-Zustimmung**

- [Erstellen einer App-Registrierung](https://docs.microsoft.com/graph/api/application-post-applications) – In diesem Artikel erfahren Sie, wie Sie ein neues Anwendungsobjekt erstellen.
- [Aktualisieren einer App-Registrierung – API-Berechtigungen](https://docs.microsoft.com/graph/api/application-update) – In diesem Artikel erfahren Sie, wie Sie die Eigenschaften eines Anwendungsobjekts aktualisieren.
- [Administratorzuwilligung](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) bereitstellen – Für die Zustimmung und Zustimmung des Administrator im Allgemeinen müssen wir verlangen, dass ein Administrator explizit seine Zustimmung erteilt.
- [RBAC (Beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Rollenverwaltungscontainer für einheitliche Rollendefinitionen und Rollenzuweisungen für Microsoft 365-RBAC-Anbieter, die mehrere Prinzipale und mehrere Bereiche in einer einzelnen Rollenzuweisung unterstützen. Dies ist anders als *der rbacApplication-Ressourcentyp.* Microsoft Intune ist ein Beispiel für einen solchen RBAC-Anbieter. Eine Rollenzuweisung in Intune kann ein Array von Prinzipale und ein Array von Bereichsgruppen haben. **Dies ist in beta, was bedeutet, dass es sich noch in der Entwicklung befindet und nicht für die Verwendung in der Produktion empfohlen wird.**
