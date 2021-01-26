---
title: Abfragen der Microsoft Graph-API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950714"
---
# <a name="querying-the-microsoft-graph-api"></a>Abfragen der Microsoft Graph-API

Dieses Thema kann auch für Entwickler gelten, die weiterhin die Azure AD Graph-API verwenden. Es wird jedoch **dringend** empfohlen, Microsoft Graph für alle Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.

**Authentifizierungs- oder Autorisierungsprobleme**

- Wenn Ihre  App keine Token zum Aufrufen von Microsoft Graph abrufen kann, wählen Sie "Problem beim Abrufen eines Zugriffstokens **(Authentifizierung)** Microsoft Graph-Kategorie" aus, um spezifischere Hilfe und Support zu diesem Thema zu erhalten.
- Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler** empfängt, wählen Sie die Microsoft Graph-API-Kategorie "Zugriff verweigert" **(Autorisierung)** aus, um spezifischere Hilfe und Support zu diesem Thema zu erhalten.

**Ich möchte Microsoft Graph verwenden, aber nicht sicher, wo ich beginnen soll**

Weitere Informationen zu Microsoft Graph finden Sie unter:

- [Übersicht über Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Übersicht über Identitäts- und Zugriffsverwaltung in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Erste Schritte beim Erstellen von Microsoft Graph-Apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demo-Mandanten

**Ich möchte Microsoft Graph verwenden, aber unterstützt es die v1.0-Verzeichnis-APIs, die ich benötigt?**

Microsoft Graph ist die empfohlene API für Verzeichnis-, Identitäts- und Zugriffsverwaltung. Es gibt jedoch immer noch einige Lücken zwischen den Möglichen in Azure AD Graph und Microsoft Graph. Lesen Sie die folgenden Artikel, in denen die aktuellen Unterschiede hervorgehoben werden, die Ihnen bei Ihrer Wahl helfen:

- [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodenunterschiede zwischen Azure AD und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Beim Abfragen des *Benutzerobjekts* fehlen viele seiner Eigenschaften.**

`GET https://graph.microsoft.com/v1.0/users` gibt nur 11 Eigenschaften zurück, da Microsoft Graph automatisch einen Standardsatz von *Benutzereigenschaften* auswählt, der zurückgegeben werden soll. Wenn Sie weitere *Benutzereigenschaften benötigen,* verwenden $select, um die Eigenschaften zu wählen, die Ihre Anwendung benötigt. Testen Sie es zuerst in **Microsoft Graph Explorer.**

**Einige Benutzereigenschaftswerte sind *NULL,* obwohl ich weiß, dass sie festgelegt sind.**

Die wahrscheinlichste Erklärung ist, dass der Anwendung die Berechtigung *User.ReadBasic.All erteilt* wurde. Dadurch kann die Anwendung eine begrenzte Anzahl von Benutzereigenschaften lesen und alle anderen Eigenschaften als NULL zurückgeben, auch wenn sie zuvor festgelegt wurden. Versuchen Sie stattdessen, der Anwendung die Berechtigung *User.Read.All* zu erteilen.

Weitere Informationen finden Sie unter [Microsoft Graph-Benutzerberechtigungen.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**I'm having trouble using OData query parameters to filter data in my requests**

Während Microsoft Graph eine vielzahl von OData-Abfrageparametern unterstützt, werden viele dieser Parameter von Verzeichnisdiensten (Ressourcen, die von *directoryObject* erben) in Microsoft Graph nicht vollständig unterstützt. Die gleichen Einschränkungen, die in Azure AD Graph vorhanden waren, bleiben in Microsoft Graph zum größten Teil bestehen:

1. **Nicht unterstützt:**$count, $search und $filter *null-* oder *nicht null-Werte*
2. **Nicht unterstützt:**$filter auf bestimmte Eigenschaften anwenden (siehe Ressourcenthemen, in denen Eigenschaften filterbar sind)
3. **Nicht unterstützt:** Auslagerung, Filterung und Sortierung gleichzeitig
4. **Nicht unterstützt:** Filtern nach einer Beziehung. Suchen Sie beispielsweise alle Mitglieder der Technischen Gruppe, die sich in Großbritannien befinden.
5. **Teilweise Unterstützung:**$orderby *für Benutzer* (nur displayName und userPrincipalName) und *Gruppe*
6. **Partielle Unterstützung:**$filter (unterstützt nur *eq*, *startswith* *oder* *und* eingeschränkte beliebige *)* unterstützung, $expand (das Erweitern der Beziehungen eines einzelnen Objekts gibt alle Beziehungen zurück, aber das Erweitern einer Auflistung von Objektbeziehungen ist begrenzt)

Weitere Informationen finden Sie unter ["Anpassen von Antworten mit Abfrageparametern".](https://docs.microsoft.com/graph/query-parameters)

**Die API, die ich aufrufe, funktioniert nicht– wo kann ich weitere Tests durchführen?**

**Microsoft Graph Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder einem Demo-Mandanten, und sehen Sie sich auch die **Beispielabfragen** in Microsoft Graph Explorer an.

**Wenn ich datenabfrage, sieht es so aus, als würde ich ein unvollständiges Datenset zurückerst**

Wenn Sie eine Sammlung abfragen (z. B. *Benutzer),* verwendet Microsoft Graph serverseitige Seitenbeschränkungen, sodass Ergebnisse immer mit einer Standardseitengröße zurückgegeben werden. Ihre App sollte immer erwarten, dass sie sammlungen, die vom Dienst zurückgegeben werden, durchseiten.

Weitere Informationen finden Sie unter:

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging der Microsoft Graph-Daten in Ihrer App](https://docs.microsoft.com/graph/paging)

**Meine App ist zu langsam und wird ebenfalls gedrosselt. Welche Verbesserungen kann ich erzielen?**

Je nach Szenario stehen Ihnen eine Vielzahl verschiedener Optionen zur Verfügung, um die Leistung ihrer Anwendung zu drosseln und in einigen Fällen weniger anfällig für eine Einschränkung durch den Dienst (wenn Sie zu viele Aufrufe ausführen).

Weitere Informationen finden Sie unter:

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batchverarbeitungsanforderungen](https://docs.microsoft.com/graph/json-batching)
- [Nachverfolgen von Änderungen über eine Deltaabfrage](https://docs.microsoft.com/graph/delta-query-overview)
- [Erhalten von Benachrichtigungen über Änderungen über Webhooks](https://docs.microsoft.com/graph/webhooks)
- [Einschränkungsleitfaden](https://docs.microsoft.com/graph/throttling)

**Wo finde ich weitere Informationen zu Fehlern und bekannten Problemen?**

- [Microsoft Graph– Fehlerantwortinformationen](https://docs.microsoft.com/graph/errors)
- [Bekannte Probleme in Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Wo kann ich den Status der Dienstverfügbarkeit und -konnektivität überprüfen?**

Die Verfügbarkeit und Konnektivität der zugrunde liegenden Dienste, auf die über Microsoft Graph zugegriffen werden kann, kann sich auf die allgemeine Verfügbarkeit und Leistung von Microsoft Graph auswirken.

- Überprüfen Sie für den Azure Active Directory-Dienststatus den Status von **Sicherheits- und Identitätsdiensten,** die auf der [Azure-Statusseite aufgeführt sind.](https://azure.microsoft.com/status/)
- Überprüfen Sie bei Office-Diensten, die zu Microsoft Graph beitragen, den Status von Diensten, die im [Office Service Health Dashboard aufgeführt sind.](https://portal.office.com/adminportal/home#/servicehealth)
