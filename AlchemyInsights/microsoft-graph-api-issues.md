---
title: Probleme mit der Microsoft Graph-API
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716198"
---
# <a name="microsoft-graph-api-issues"></a>Probleme mit der Microsoft Graph-API

Dieses Thema kann auch für Entwickler gelten, die weiterhin Azure AD Graph-API verwenden. Es wird jedoch **dringend empfohlen,** Microsoft Graph für alle Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.

**Authentifizierungs- oder Autorisierungsprobleme**

- Wenn Ihre  App keine Token zum Aufrufen von Microsoft Graph erwerben kann, wählen Sie Problem mit dem Abrufen eines Zugriffstokens **(Authentifizierung)** Microsoft Graph-Kategorie aus, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.
- Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler** erhält, wählen Sie die Microsoft Graph-API-Kategorie Abrufen eines Zugriffs verweigerten Fehlers **(Autorisierung)** aus, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.

**Ich möchte Microsoft Graph verwenden, aber nicht sicher, wo ich beginnen soll**

- [Übersicht über Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Übersicht über die Identitäts- und Zugriffsverwaltung in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Erste Schritte beim Erstellen von Microsoft Graph-Apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demo-Mandanten

**Ich möchte Microsoft Graph verwenden, aber unterstützt es die v1.0-Verzeichnis-APIs, die ich brauche?**

Microsoft Graph ist die empfohlene API für die Verzeichnis-, Identitäts- und Zugriffsverwaltung. Es gibt jedoch noch einige Lücken zwischen den Möglichen in Azure AD Graph und Microsoft Graph. Lesen Sie die folgenden Artikel, in denen die aktuellen Unterschiede hervorgehoben werden, die Ihnen bei ihrer Auswahl helfen:

- [Unterschiede beim Ressourcentyp zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodenunterschiede zwischen Azure AD und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Die API, die ich aufrufe, funktioniert nicht – wo kann ich weitere Tests durchführen?**

**Microsoft Graph Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder Demo-Mandanten, und sehen Sie sich auch die **Beispielabfragen** im Microsoft Graph Explorer an.

**Meine App ist zu langsam und wird ebenfalls gedrosselt. Welche Verbesserungen kann ich erzielen?**

Je nach Szenario stehen Ihnen eine Vielzahl von Optionen zur Verfügung, um Ihre Anwendung effizienter und in einigen Fällen weniger anfällig für die Einschränkung durch den Dienst zu machen (wenn Sie zu viele Anrufe ausführen).

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batchanforderungen](https://docs.microsoft.com/graph/json-batching)
- [Nachverfolgen von Änderungen über delta-Abfrage](https://docs.microsoft.com/graph/delta-query-overview)
- [Über Webhooks über Änderungen benachrichtigt werden](https://docs.microsoft.com/graph/webhooks)
- [Einschränkungsleitfaden](https://docs.microsoft.com/graph/throttling)

**Wo finde ich weitere Informationen zu Fehlern und bekannten Problemen?**

- [Microsoft Graph-Fehlerantwortinformationen](https://docs.microsoft.com/graph/errors)
- [Bekannte Probleme in Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Wo kann ich den Status der Dienstverfügbarkeit und -konnektivität überprüfen?**

Die Verfügbarkeit und Konnektivität der zugrunde liegenden Dienste, auf die über Microsoft Graph zugegriffen werden kann, kann sich auf die Allgemeine Verfügbarkeit und Leistung von Microsoft Graph auswirken.

- Überprüfen Sie für die Integrität des Azure Active Directory-Diensts den Status von **Sicherheits- und Identitätsdiensten,** die auf der [Azure-Statusseite aufgeführt sind.](https://azure.microsoft.com/status/)
- Überprüfen Sie für Office-Dienste, die zu Microsoft Graph beitragen, den Status von Diensten, die im [Office Service Health Dashboard aufgeführt sind.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph-Autorisierungsfehler können auf verschiedene Probleme resultieren, von denen die meisten einen Fehler 401 oder 403 generieren. Die folgenden Beispiele können zu Autorisierungsfehlern führen:

- Falsche [Flüsse für den Erwerb von Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Schlecht konfigurierte [Berechtigungsumfänge](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Fehlende [Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Ende der Unterstützung von Azure Active Directory-Authentifizierungsbibliothek (ADAL) und Azure AD Graph-API (AAD Graph)_* _

_*Ab dem 30. Juni 2020** werden ADAL und Azure AD Graph keine neuen Features mehr hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.

**Ab dem 30. Juni 2022** beenden wir die Unterstützung für ADAL und Azure AD Graph und stellen keine technischen Support- oder Sicherheitsupdates mehr bereit.

Apps, die ADAL auf vorhandenen Betriebssystemversionen verwenden, funktionieren nach dieser Zeit weiterhin, erhalten jedoch keinen *technischen Support oder Sicherheitsupdates.*

Apps, die Azure AD Graph nach dieser Zeit verwenden, erhalten möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL-Migration**

Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.

Wenn Sie Microsoft-Apps verwenden, sollten Sie wissen, dass Microsoft seine Anwendungen bis zum Ende des Supporttermins zu MSAL migriert, um sicherzustellen, dass sie von den fortlaufenden Verbesserungen von Sicherheit und Funktionen von MSAL profitieren.

1. [Häufig gestellte Fragen zu ADAL lesen](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Wenn Sie hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir, dass Sie den Quellcode Ihrer Apps überprüfen und ggf. alle ISVs oder App-Anbieter erreichen. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Befolgen Sie für Anwendungen, die Azure AD Graph verwenden, unsere Anleitungen zum Migrieren von [Azure AD Graph-Apps zu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Unsere Migrationscheckliste stellt einen guten Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen auch eine Liste aller AAD Graph-Nutzungen in Ihrem Mandanten bereitstellen.
3. Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. Die [Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) listet die Berechtigungen auf, die den einzelnen Hauptsatz von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.
