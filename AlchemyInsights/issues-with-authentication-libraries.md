---
title: Probleme mit Authentifizierungsbibliotheken
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037215"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="a29bc-102">Probleme mit Authentifizierungsbibliotheken</span><span class="sxs-lookup"><span data-stu-id="a29bc-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="a29bc-103">[Microsoft Identity Platform-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) listen von Microsoft unterstützte und kompatible Client- und Middlewarebibliotheken auf.</span><span class="sxs-lookup"><span data-stu-id="a29bc-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="a29bc-104">Die Microsoft Authentication Library (MSAL) unterstützt mehrere [Authentifizierungsflüsse](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) für die Verwendung in verschiedenen Anwendungsszenarien.</span><span class="sxs-lookup"><span data-stu-id="a29bc-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="a29bc-105">Zum Authentifizieren und Erwerben von Token initialisieren Sie eine neue öffentliche oder vertrauliche Clientanwendung in Ihrem Code.</span><span class="sxs-lookup"><span data-stu-id="a29bc-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="a29bc-106">Sie können mehrere Konfigurationsoptionen festlegen, wenn Sie die Client-App in der Microsoft Authentication Library (MSAL) initialisieren.</span><span class="sxs-lookup"><span data-stu-id="a29bc-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="a29bc-107">Weitere Informationen finden Sie unter [Anwendungskonfigurationsoptionen.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="a29bc-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="a29bc-108">**Ende der Unterstützung für Azure Active Directory Authentication Library (ADAL) und Azure AD Graph-API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="a29bc-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="a29bc-109">**Ab dem 30. Juni 2020** werden ADAL und Azure AD Graph keine neuen Features mehr hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a29bc-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="a29bc-110">Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.</span><span class="sxs-lookup"><span data-stu-id="a29bc-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="a29bc-111">**Ab dem 30. Juni 2022** beenden wir die Unterstützung für ADAL und Azure AD Graph und stellen keine technischen Support- oder Sicherheitsupdates mehr bereit.</span><span class="sxs-lookup"><span data-stu-id="a29bc-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="a29bc-112">Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren nach dieser Zeit weiterhin, erhalten jedoch keinen *technischen Support oder Sicherheitsupdates.*</span><span class="sxs-lookup"><span data-stu-id="a29bc-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="a29bc-113">Apps, die Azure AD Graph nach dieser Zeit verwenden, erhalten möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="a29bc-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="a29bc-114">**ADAL Migration**</span><span class="sxs-lookup"><span data-stu-id="a29bc-114">**ADAL Migration**</span></span>

<span data-ttu-id="a29bc-115">Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.</span><span class="sxs-lookup"><span data-stu-id="a29bc-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="a29bc-116">Wenn Sie Microsoft Apps verwenden, wissen Sie, dass Microsoft seine Anwendungen bis zum Ende des Supporttermins zu MSAL migriert, um sicherzustellen, dass sie von den fortlaufenden Sicherheits- und Funktionsverbesserungen von MSAL profitieren.</span><span class="sxs-lookup"><span data-stu-id="a29bc-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="a29bc-117">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="a29bc-117">For more information, see:</span></span>

1. [<span data-ttu-id="a29bc-118">Häufig gestellte Fragen zu ADAL lesen</span><span class="sxs-lookup"><span data-stu-id="a29bc-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="a29bc-119">Informationen zum Migrieren von Apps nach Plattform</span><span class="sxs-lookup"><span data-stu-id="a29bc-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="a29bc-120">Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und ggf. alle ISVs oder App-Anbieter zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="a29bc-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a29bc-121">Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="a29bc-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="a29bc-122">**AAD Graph-Migration**</span><span class="sxs-lookup"><span data-stu-id="a29bc-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="a29bc-123">Befolgen Sie für Anwendungen, die Azure AD Graph verwenden, unsere Anleitungen zum Migrieren [von Azure AD Graph-Apps zu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="a29bc-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="a29bc-124">Unsere Migrationscheckliste bietet einen Einstiegspunkt.</span><span class="sxs-lookup"><span data-stu-id="a29bc-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="a29bc-125">In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden.</span><span class="sxs-lookup"><span data-stu-id="a29bc-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="a29bc-126">Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen.</span><span class="sxs-lookup"><span data-stu-id="a29bc-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a29bc-127">Der Support von Microsoft kann Ihnen auch eine Liste aller AAD Graph-Nutzungen in Ihrem Mandanten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="a29bc-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="a29bc-128">Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen.</span><span class="sxs-lookup"><span data-stu-id="a29bc-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="a29bc-129">In [der Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) werden die Berechtigungen aufgeführt, die den einzelnen Hauptsatz von Microsoft Graph-APIs zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="a29bc-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="a29bc-130">Es enthält auch Anleitungen zur Verwendung der Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="a29bc-130">It also provides guidance about how to use the permissions.</span></span>
