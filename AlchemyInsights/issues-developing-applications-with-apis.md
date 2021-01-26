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
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="21550-102">Probleme beim Entwickeln von Anwendungen mit APIs</span><span class="sxs-lookup"><span data-stu-id="21550-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="21550-103">Informationen zur Verwendung der Azure Active Directory Graph-API finden Sie im [Schnellstarthandbuch zur Azure AD Graph-API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) oder in der referenzdokumentation zur interaktiven Azure AD [Graph-API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="21550-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="21550-104">**Ende der Unterstützung für Azure Active Directory Authentication Library (ADAL) und Azure AD Graph-API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="21550-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="21550-105">**Ab dem 30. Juni 2020** werden ADAL und Azure AD Graph keine neuen Features mehr hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="21550-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="21550-106">Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, aber keine Funktionsupdates mehr bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="21550-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="21550-107">**Ab dem 30. Juni 2022** beenden wir die Unterstützung für ADAL und Azure AD Graph und stellen keine technischen Support- oder Sicherheitsupdates mehr bereit.</span><span class="sxs-lookup"><span data-stu-id="21550-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="21550-108">Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren nach dieser Zeit weiterhin, erhalten jedoch keinen technischen Support oder Sicherheitsupdates.</span><span class="sxs-lookup"><span data-stu-id="21550-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="21550-109">Apps, die Azure AD Graph nach dieser Zeit verwenden, erhalten möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="21550-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="21550-110">**ADAL Migration**</span><span class="sxs-lookup"><span data-stu-id="21550-110">**ADAL Migration**</span></span>

<span data-ttu-id="21550-111">Es wird empfohlen, auf die [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)zu aktualisieren, die über die neuesten Features und Sicherheitsupdates verfügt.</span><span class="sxs-lookup"><span data-stu-id="21550-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="21550-112">Wenn Sie Microsoft Apps verwenden, wissen Sie, dass Microsoft seine Anwendungen bis zum Ende des Supporttermins zu MSAL migriert, um sicherzustellen, dass sie von den fortlaufenden Sicherheits- und Funktionsverbesserungen von MSAL profitieren.</span><span class="sxs-lookup"><span data-stu-id="21550-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="21550-113">[Lesen Sie die häufig gestellten Fragen zu ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="21550-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="21550-114">[Erfahren Sie, wie Sie Apps pro](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)Plattform migrieren.</span><span class="sxs-lookup"><span data-stu-id="21550-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="21550-115">Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und ggf. alle ISVs oder App-Anbieter zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="21550-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="21550-116">Der Support von Microsoft kann Ihnen auch eine Liste aller Nicht-Microsoft-ADAL-Apps in Ihrem Mandanten zur Verfügung stellen.</span><span class="sxs-lookup"><span data-stu-id="21550-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="21550-117">**AAD Graph Migration**</span><span class="sxs-lookup"><span data-stu-id="21550-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="21550-118">Befolgen Sie für Anwendungen, die Azure AD Graph verwenden, unsere Anleitungen zum Migrieren [von Azure AD Graph-Apps zu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="21550-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="21550-119">[Unsere Migrationscheckliste bietet einen Einstiegspunkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="21550-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="21550-120">Ihr Azure-App-Registrierungsportal zeigt, welche Anwendungen AAD Graph verwenden.</span><span class="sxs-lookup"><span data-stu-id="21550-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="21550-121">Es wird empfohlen, den Quellcode Ihrer Apps zu überprüfen und ggf. alle ISVs oder App-Anbieter zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="21550-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="21550-122">Der Support von Microsoft kann Ihnen auch eine Liste aller AAD Graph-Nutzungen in Ihrem Mandanten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="21550-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="21550-123">Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen.</span><span class="sxs-lookup"><span data-stu-id="21550-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="21550-124">In [der Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) werden die Berechtigungen aufgeführt, die den einzelnen Hauptsatz von Microsoft Graph-APIs zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="21550-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="21550-125">Es enthält auch Anleitungen zur Verwendung der Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="21550-125">It also provides guidance about how to use the permissions.</span></span>
