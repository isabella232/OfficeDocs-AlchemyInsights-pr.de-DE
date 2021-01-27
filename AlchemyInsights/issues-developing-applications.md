---
title: Probleme bei der Entwicklung von Anwendungen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950733"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="8e81a-102">Probleme bei der Entwicklung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="8e81a-102">Issues developing applications</span></span>

<span data-ttu-id="8e81a-103">Informationen zur Behebung der häufigsten Probleme beim Entwickeln von Azure Active Directory (AD)-Apps finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="8e81a-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="8e81a-104">Es gibt Probleme beim Anmelden bei Anwendungen nur mit dem Chrome-Browser</span><span class="sxs-lookup"><span data-stu-id="8e81a-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="8e81a-105">Ich weiß nicht, wie ich die Standardeinstellungen für die Gültigkeitsdauer von Token für meine Anwendung ändern kann</span><span class="sxs-lookup"><span data-stu-id="8e81a-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="8e81a-106">Mir ist unklar, wie die Zustimmung für Anwendungen funktioniert</span><span class="sxs-lookup"><span data-stu-id="8e81a-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="8e81a-107">Ich weiß nicht, wie Berechtigungen für meine Anwendung erteilt werden</span><span class="sxs-lookup"><span data-stu-id="8e81a-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="8e81a-108">Mir ist der Unterschied zwischen delegierten und Anwendungsberechtigungen nicht klar</span><span class="sxs-lookup"><span data-stu-id="8e81a-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="8e81a-109">\***Ende der Unterstützung von Azure Active Directory-Authentifizierungsbibliothek (ADAL) und Azure AD Graph-API (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="8e81a-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="8e81a-110">Ab dem 30. Juni 2020 werden der Azure Active Directory-Authentifizierungsbibliothek (ADAL) und der Azure AD Graph-API (AAD Graph) keine neuen Features mehr hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="8e81a-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="8e81a-111">Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.</span><span class="sxs-lookup"><span data-stu-id="8e81a-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="8e81a-112">Ab dem 30. Juni 2022 werden wir den Support für ADAL und Azure AD Graph beenden und keinen technischen Support oder Sicherheitsupdates mehr dafür bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="8e81a-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="8e81a-113">Dies wird folgende Auswirkungen haben:</span><span class="sxs-lookup"><span data-stu-id="8e81a-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="8e81a-114">Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="8e81a-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="8e81a-115">Apps, die AAD Graph nach diesem Zeitpunkt verwenden, werden keine Antworten mehr vom AAD Graph-Endpunkt erhalten.</span><span class="sxs-lookup"><span data-stu-id="8e81a-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="8e81a-116">_ *ADAL-Migration*\*</span><span class="sxs-lookup"><span data-stu-id="8e81a-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="8e81a-117">Wenn Sie Microsoft-Apps verwenden, wird ein Update auf die Microsoft-Authentifizierungsbibliothek (MSAL) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.</span><span class="sxs-lookup"><span data-stu-id="8e81a-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="8e81a-118">Diese Empfehlung steht in Zusammenhang mit dem Beginn der Migration der eigenen Anwendungen durch Microsoft nach MSAL bis zum Enddatum des Supports.</span><span class="sxs-lookup"><span data-stu-id="8e81a-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="8e81a-119">Durch die Migration der eigenen Apps durch Microsoft zu MSAL wird sichergestellt, dass sie von den ständigen Sicherheits- und Featureverbesserungen für MSAL profitieren.</span><span class="sxs-lookup"><span data-stu-id="8e81a-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="8e81a-120">Häufig gestellte Fragen zu ADAL lesen</span><span class="sxs-lookup"><span data-stu-id="8e81a-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="8e81a-121">Informationen zum Migrieren von Apps nach Plattform</span><span class="sxs-lookup"><span data-stu-id="8e81a-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="8e81a-122">Wenn Sie ermitteln müssen, welche Ihrer Apps ADAL verwenden, und dabei Hilfe benötigen, empfehlen wir, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an unabhängige Softwareanbieter (ISVs) oder App-Anbieter zu wenden.</span><span class="sxs-lookup"><span data-stu-id="8e81a-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="8e81a-123">Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="8e81a-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8e81a-124">**AAD Graph-Migration**</span><span class="sxs-lookup"><span data-stu-id="8e81a-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="8e81a-125">Folgen Sie bei Anwendungen, die AAD Graph verwenden, unseren Anweisungen zum Migrieren von Azure AD Graph-Apps zu Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8e81a-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="8e81a-126">[Unsere Migrationscheckliste stellt einen guten Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="8e81a-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="8e81a-127">In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden.</span><span class="sxs-lookup"><span data-stu-id="8e81a-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8e81a-128">Es wird empfohlen, den Quellcode all Ihrer Apps zu überprüfen, und sich ggf. mit unabhängigen Softwareanbietern (ISVs) oder App-Anbietern in Verbindung zu setzen.</span><span class="sxs-lookup"><span data-stu-id="8e81a-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="8e81a-129">Der Microsoft-Support kann Ihnen darüber hinaus Informationen zur AAD Graph-Nutzung in Ihrem Mandanten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="8e81a-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







