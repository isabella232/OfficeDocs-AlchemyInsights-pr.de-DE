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
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="51d63-102">Abfragen der Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="51d63-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="51d63-103">Dieses Thema kann auch für Entwickler gelten, die weiterhin die Azure AD Graph-API verwenden.</span><span class="sxs-lookup"><span data-stu-id="51d63-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="51d63-104">Es wird jedoch **dringend** empfohlen, Microsoft Graph für alle Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="51d63-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="51d63-105">**Authentifizierungs- oder Autorisierungsprobleme**</span><span class="sxs-lookup"><span data-stu-id="51d63-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="51d63-106">Wenn Ihre  App keine Token zum Aufrufen von Microsoft Graph abrufen kann, wählen Sie "Problem beim Abrufen eines Zugriffstokens **(Authentifizierung)** Microsoft Graph-Kategorie" aus, um spezifischere Hilfe und Support zu diesem Thema zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="51d63-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="51d63-107">Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler** empfängt, wählen Sie die Microsoft Graph-API-Kategorie "Zugriff verweigert" **(Autorisierung)** aus, um spezifischere Hilfe und Support zu diesem Thema zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="51d63-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="51d63-108">**Ich möchte Microsoft Graph verwenden, aber nicht sicher, wo ich beginnen soll**</span><span class="sxs-lookup"><span data-stu-id="51d63-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="51d63-109">Weitere Informationen zu Microsoft Graph finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="51d63-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="51d63-110">Übersicht über Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="51d63-111">Übersicht über Identitäts- und Zugriffsverwaltung in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="51d63-112">Erste Schritte beim Erstellen von Microsoft Graph-Apps</span><span class="sxs-lookup"><span data-stu-id="51d63-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="51d63-113">**Microsoft Graph Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demo-Mandanten</span><span class="sxs-lookup"><span data-stu-id="51d63-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="51d63-114">**Ich möchte Microsoft Graph verwenden, aber unterstützt es die v1.0-Verzeichnis-APIs, die ich benötigt?**</span><span class="sxs-lookup"><span data-stu-id="51d63-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="51d63-115">Microsoft Graph ist die empfohlene API für Verzeichnis-, Identitäts- und Zugriffsverwaltung.</span><span class="sxs-lookup"><span data-stu-id="51d63-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="51d63-116">Es gibt jedoch immer noch einige Lücken zwischen den Möglichen in Azure AD Graph und Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="51d63-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="51d63-117">Lesen Sie die folgenden Artikel, in denen die aktuellen Unterschiede hervorgehoben werden, die Ihnen bei Ihrer Wahl helfen:</span><span class="sxs-lookup"><span data-stu-id="51d63-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="51d63-118">Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="51d63-119">Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="51d63-120">Methodenunterschiede zwischen Azure AD und Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="51d63-121">**Beim Abfragen des *Benutzerobjekts* fehlen viele seiner Eigenschaften.**</span><span class="sxs-lookup"><span data-stu-id="51d63-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="51d63-122">`GET https://graph.microsoft.com/v1.0/users` gibt nur 11 Eigenschaften zurück, da Microsoft Graph automatisch einen Standardsatz von *Benutzereigenschaften* auswählt, der zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="51d63-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="51d63-123">Wenn Sie weitere *Benutzereigenschaften benötigen,* verwenden $select, um die Eigenschaften zu wählen, die Ihre Anwendung benötigt.</span><span class="sxs-lookup"><span data-stu-id="51d63-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="51d63-124">Testen Sie es zuerst in **Microsoft Graph Explorer.**</span><span class="sxs-lookup"><span data-stu-id="51d63-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="51d63-125">**Einige Benutzereigenschaftswerte sind *NULL,* obwohl ich weiß, dass sie festgelegt sind.**</span><span class="sxs-lookup"><span data-stu-id="51d63-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="51d63-126">Die wahrscheinlichste Erklärung ist, dass der Anwendung die Berechtigung *User.ReadBasic.All erteilt* wurde.</span><span class="sxs-lookup"><span data-stu-id="51d63-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="51d63-127">Dadurch kann die Anwendung eine begrenzte Anzahl von Benutzereigenschaften lesen und alle anderen Eigenschaften als NULL zurückgeben, auch wenn sie zuvor festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="51d63-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="51d63-128">Versuchen Sie stattdessen, der Anwendung die Berechtigung *User.Read.All* zu erteilen.</span><span class="sxs-lookup"><span data-stu-id="51d63-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="51d63-129">Weitere Informationen finden Sie unter [Microsoft Graph-Benutzerberechtigungen.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="51d63-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="51d63-130">**I'm having trouble using OData query parameters to filter data in my requests**</span><span class="sxs-lookup"><span data-stu-id="51d63-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="51d63-131">Während Microsoft Graph eine vielzahl von OData-Abfrageparametern unterstützt, werden viele dieser Parameter von Verzeichnisdiensten (Ressourcen, die von *directoryObject* erben) in Microsoft Graph nicht vollständig unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51d63-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="51d63-132">Die gleichen Einschränkungen, die in Azure AD Graph vorhanden waren, bleiben in Microsoft Graph zum größten Teil bestehen:</span><span class="sxs-lookup"><span data-stu-id="51d63-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="51d63-133">**Nicht unterstützt:**$count, $search und $filter *null-* oder *nicht null-Werte*</span><span class="sxs-lookup"><span data-stu-id="51d63-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="51d63-134">**Nicht unterstützt:**$filter auf bestimmte Eigenschaften anwenden (siehe Ressourcenthemen, in denen Eigenschaften filterbar sind)</span><span class="sxs-lookup"><span data-stu-id="51d63-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="51d63-135">**Nicht unterstützt:** Auslagerung, Filterung und Sortierung gleichzeitig</span><span class="sxs-lookup"><span data-stu-id="51d63-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="51d63-136">**Nicht unterstützt:** Filtern nach einer Beziehung.</span><span class="sxs-lookup"><span data-stu-id="51d63-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="51d63-137">Suchen Sie beispielsweise alle Mitglieder der Technischen Gruppe, die sich in Großbritannien befinden.</span><span class="sxs-lookup"><span data-stu-id="51d63-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="51d63-138">**Teilweise Unterstützung:**$orderby *für Benutzer* (nur displayName und userPrincipalName) und *Gruppe*</span><span class="sxs-lookup"><span data-stu-id="51d63-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="51d63-139">**Partielle Unterstützung:**$filter (unterstützt nur *eq*, *startswith* *oder* *und* eingeschränkte beliebige *)* unterstützung, $expand (das Erweitern der Beziehungen eines einzelnen Objekts gibt alle Beziehungen zurück, aber das Erweitern einer Auflistung von Objektbeziehungen ist begrenzt)</span><span class="sxs-lookup"><span data-stu-id="51d63-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="51d63-140">Weitere Informationen finden Sie unter ["Anpassen von Antworten mit Abfrageparametern".](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="51d63-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="51d63-141">**Die API, die ich aufrufe, funktioniert nicht– wo kann ich weitere Tests durchführen?**</span><span class="sxs-lookup"><span data-stu-id="51d63-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="51d63-142">**Microsoft Graph Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder einem Demo-Mandanten, und sehen Sie sich auch die **Beispielabfragen** in Microsoft Graph Explorer an.</span><span class="sxs-lookup"><span data-stu-id="51d63-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="51d63-143">**Wenn ich datenabfrage, sieht es so aus, als würde ich ein unvollständiges Datenset zurückerst**</span><span class="sxs-lookup"><span data-stu-id="51d63-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="51d63-144">Wenn Sie eine Sammlung abfragen (z. B. *Benutzer),* verwendet Microsoft Graph serverseitige Seitenbeschränkungen, sodass Ergebnisse immer mit einer Standardseitengröße zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="51d63-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="51d63-145">Ihre App sollte immer erwarten, dass sie sammlungen, die vom Dienst zurückgegeben werden, durchseiten.</span><span class="sxs-lookup"><span data-stu-id="51d63-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="51d63-146">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="51d63-146">For more information, see:</span></span>

- [<span data-ttu-id="51d63-147">Bewährte Methoden für Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="51d63-148">Paging der Microsoft Graph-Daten in Ihrer App</span><span class="sxs-lookup"><span data-stu-id="51d63-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="51d63-149">**Meine App ist zu langsam und wird ebenfalls gedrosselt. Welche Verbesserungen kann ich erzielen?**</span><span class="sxs-lookup"><span data-stu-id="51d63-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="51d63-150">Je nach Szenario stehen Ihnen eine Vielzahl verschiedener Optionen zur Verfügung, um die Leistung ihrer Anwendung zu drosseln und in einigen Fällen weniger anfällig für eine Einschränkung durch den Dienst (wenn Sie zu viele Aufrufe ausführen).</span><span class="sxs-lookup"><span data-stu-id="51d63-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="51d63-151">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="51d63-151">To learn more, see:</span></span>

- [<span data-ttu-id="51d63-152">Bewährte Methoden für Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="51d63-153">Batchverarbeitungsanforderungen</span><span class="sxs-lookup"><span data-stu-id="51d63-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="51d63-154">Nachverfolgen von Änderungen über eine Deltaabfrage</span><span class="sxs-lookup"><span data-stu-id="51d63-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="51d63-155">Erhalten von Benachrichtigungen über Änderungen über Webhooks</span><span class="sxs-lookup"><span data-stu-id="51d63-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="51d63-156">Einschränkungsleitfaden</span><span class="sxs-lookup"><span data-stu-id="51d63-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="51d63-157">**Wo finde ich weitere Informationen zu Fehlern und bekannten Problemen?**</span><span class="sxs-lookup"><span data-stu-id="51d63-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="51d63-158">Microsoft Graph– Fehlerantwortinformationen</span><span class="sxs-lookup"><span data-stu-id="51d63-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="51d63-159">Bekannte Probleme in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51d63-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="51d63-160">**Wo kann ich den Status der Dienstverfügbarkeit und -konnektivität überprüfen?**</span><span class="sxs-lookup"><span data-stu-id="51d63-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="51d63-161">Die Verfügbarkeit und Konnektivität der zugrunde liegenden Dienste, auf die über Microsoft Graph zugegriffen werden kann, kann sich auf die allgemeine Verfügbarkeit und Leistung von Microsoft Graph auswirken.</span><span class="sxs-lookup"><span data-stu-id="51d63-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="51d63-162">Überprüfen Sie für den Azure Active Directory-Dienststatus den Status von **Sicherheits- und Identitätsdiensten,** die auf der [Azure-Statusseite aufgeführt sind.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="51d63-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="51d63-163">Überprüfen Sie bei Office-Diensten, die zu Microsoft Graph beitragen, den Status von Diensten, die im [Office Service Health Dashboard aufgeführt sind.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="51d63-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
