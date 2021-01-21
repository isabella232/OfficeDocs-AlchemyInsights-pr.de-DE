---
title: Konfigurieren und Verlängern der Tokengültigkeitsdauer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911996"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="893a1-102">Konfigurieren und Verlängern der Tokengültigkeitsdauer</span><span class="sxs-lookup"><span data-stu-id="893a1-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="893a1-103">Sie können die Gültigkeitsdauer für von Microsoft Identity Platform ausgestellte Zugriffs-, SAML- oder ID-Tokens angeben.</span><span class="sxs-lookup"><span data-stu-id="893a1-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="893a1-104">Sie können die Tokengültigkeitsdauer für alle Apps in Ihrer Organisation festlegen, für eine mehrinstanzfähige (multiorganisatorische) Anwendung oder für einen bestimmten Dienstprinzipal in Ihrer Organisation.</span><span class="sxs-lookup"><span data-stu-id="893a1-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="893a1-105">Weitere Informationen finden Sie unter [Konfigurierbare Tokengültigkeitsdauer](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="893a1-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="893a1-106">Beispiele finden Sie unter [Beispielen zur Konfiguration der Tokengültigkeitsdauer](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="893a1-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="893a1-107">Wie Sie die Gültigkeitsdauer und Kompatibilität eines Tokens in Azure Active Directory B2C (Azure AD B2C) konfigurieren können, erfahren Sie unter [Konfigurieren von Token in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="893a1-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="893a1-108">Der Artikel [Konfigurieren des Sitzungsverhaltens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beschreibt die in Azure AD B2C verwendeten Methoden zum einmaligen Anmelden (Single Sign-On, SSO) und bietet Unterstützung bei der Auswahl der am besten geeigneten SSO-Methode bei der Konfiguration Ihrer Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="893a1-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="893a1-109">**Wie lange bleiben die Token bestehen? Wie lange sind sie gültig?**</span><span class="sxs-lookup"><span data-stu-id="893a1-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="893a1-110">Die Tokengültigkeitsdauer beträgt 1 Stunde und die Sitzungsgültigkeitsdauer beträgt 24 Stunden.</span><span class="sxs-lookup"><span data-stu-id="893a1-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="893a1-111">Das bedeutet, dass Sie sich erneut anmelden müssen, bevor Sie ein neues Token anfordern können, wenn innerhalb von 24 Stunden keine Anforderung erfolgt ist.</span><span class="sxs-lookup"><span data-stu-id="893a1-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="893a1-112">Nach dem 30. Mai 2020 können neue Mandanten die Richtlinie „Gültigkeitsdauer konfigurierbarer Token“ nicht mehr verwenden, um Sitzungs- und Aktualisierungstoken zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="893a1-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="893a1-113">Die Einstellung erfolgt in den nächsten Monaten, was bedeutet, dass bestehende Richtlinien für Sitzungs- und Aktualisierungstokens nicht mehr berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="893a1-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="893a1-114">Sie können die Gültigkeitsdauer von Token auch nach der Einstellung noch konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="893a1-114">You can still configure access token lifetimes after the deprecation.</span></span>






