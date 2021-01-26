---
title: Probleme beim Entwickeln von Anwendungen mit APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951900"
---
# <a name="issues-developing-applications-with-apis"></a>Probleme beim Entwickeln von Anwendungen mit APIs

Informationen zur Verwendung der Azure Active Directory Graph-API finden Sie im [Schnellstarthandbuch zur Azure AD Graph-API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) oder in der referenzdokumentation zur interaktiven Azure AD [Graph-API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Ende der Unterstützung für Azure Active Directory Authentication Library (ADAL) und Azure AD Graph-API (AAD Graph)**

**Ab dem 30. Juni 2020** werden ADAL und Azure AD Graph keine neuen Features mehr hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, aber keine Funktionsupdates mehr bereitstellen.

**Ab dem 30. Juni 2022** beenden wir die Unterstützung für ADAL und Azure AD Graph und stellen keine technischen Support- oder Sicherheitsupdates mehr bereit.

Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren nach dieser Zeit weiterhin, erhalten jedoch keinen technischen Support oder Sicherheitsupdates.

Apps, die Azure AD Graph nach dieser Zeit verwenden, erhalten möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL Migration**

Es wird empfohlen, auf die [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)zu aktualisieren, die über die neuesten Features und Sicherheitsupdates verfügt.

Wenn Sie Microsoft Apps verwenden, wissen Sie, dass Microsoft seine Anwendungen bis zum Ende des Supporttermins zu MSAL migriert, um sicherzustellen, dass sie von den fortlaufenden Sicherheits- und Funktionsverbesserungen von MSAL profitieren.

1. [Lesen Sie die häufig gestellten Fragen zu ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Erfahren Sie, wie Sie Apps pro](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)Plattform migrieren.
1. Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und ggf. alle ISVs oder App-Anbieter zu erreichen. Der Support von Microsoft kann Ihnen auch eine Liste aller Nicht-Microsoft-ADAL-Apps in Ihrem Mandanten zur Verfügung stellen.

**AAD Graph Migration**

Befolgen Sie für Anwendungen, die Azure AD Graph verwenden, unsere Anleitungen zum Migrieren [von Azure AD Graph-Apps zu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Unsere Migrationscheckliste bietet einen Einstiegspunkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Ihr Azure-App-Registrierungsportal zeigt, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, den Quellcode Ihrer Apps zu überprüfen und ggf. alle ISVs oder App-Anbieter zu erreichen. Der Support von Microsoft kann Ihnen auch eine Liste aller AAD Graph-Nutzungen in Ihrem Mandanten bereitstellen.
1. Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. In [der Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) werden die Berechtigungen aufgeführt, die den einzelnen Hauptsatz von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.
