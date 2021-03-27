---
title: Erweiterte Authentifizierungskonzepte für Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398560"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="a59ea-102">Erweiterte Authentifizierungskonzepte für Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a59ea-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="a59ea-103">Nachfolgend finden Sie die erweiterten Authentifizierungskonzepte, die für Microsoft Edge gelten:</span><span class="sxs-lookup"><span data-stu-id="a59ea-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="a59ea-104">**Proaktive Authentifizierung**</span><span class="sxs-lookup"><span data-stu-id="a59ea-104">**Proactive Authentication**</span></span>

<span data-ttu-id="a59ea-105">Wenn Sie die [ProaktiveAuthEnabled-Richtlinie](https://go.microsoft.com/fwlink/?linkid=2134621) aktivieren, versucht Microsoft Edge, angemeldete Benutzer proaktiv über Microsoft-Dienste zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="a59ea-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="a59ea-106">In regelmäßigen Abständen wird ein Onlinedienst verwendet, um nach einem aktualisierten Manifest zu suchen, das die Konfiguration für die proaktive Authentifizierung enthält.</span><span class="sxs-lookup"><span data-stu-id="a59ea-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="a59ea-107">Vorteile: Die proaktive Authentifizierung ermöglicht die Authentifizierung für wichtige Dienste, z. B. die Office New Tab Page.</span><span class="sxs-lookup"><span data-stu-id="a59ea-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="a59ea-108">Wenn Bing als Suchmaschine verwendet wird, verbessert die proaktive Authentifizierung außerdem die Leistung der Adressleiste und hilft bei der Generierung von Suchergebnissen, die auf die Anforderungen Ihres Unternehmens zugeschnitten sind.</span><span class="sxs-lookup"><span data-stu-id="a59ea-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="a59ea-109">**Windows Hello CredUI für die NTLM-Authentifizierung**</span><span class="sxs-lookup"><span data-stu-id="a59ea-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="a59ea-110">Wenn einmaliges Anmelden (Single Sign-On, SSO) nicht verfügbar ist, wenn eine Website versucht, sich über den NTLM- oder Negotiate-Mechanismus beim Benutzer zu registrieren, ermöglicht dieses Feature dem Benutzer, die Anmeldeinformationen des Betriebssystems für die Website frei zu geben und die Authentifizierungsanforderungen mithilfe der Windows Hello Cred-Benutzeroberfläche zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="a59ea-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="a59ea-111">Dieser Anmeldefluss wird nur unter Windows 10 und nur für Benutzer angezeigt, die während eines NTLM oder einer Negotiate-Herausforderung keine SSO erhalten.</span><span class="sxs-lookup"><span data-stu-id="a59ea-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="a59ea-112">**Automatische Anmeldung mit gespeicherten Kennwörtern**</span><span class="sxs-lookup"><span data-stu-id="a59ea-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="a59ea-113">Benutzer, die Kennwörter in Microsoft Edge speichern, können die automatische Anmeldung bei Websites aktivieren, auf denen sie Anmeldeinformationen gespeichert haben.</span><span class="sxs-lookup"><span data-stu-id="a59ea-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="a59ea-114">Benutzer können dieses Feature in edge://settings/passwords aktivieren oder deaktivieren, und Sie können es in den [Kennwort-Manager-Richtlinien](https://go.microsoft.com/fwlink/?linkid=2134622) konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="a59ea-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
