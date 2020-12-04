---
title: Erweiterte Authentifizierungskonzepte, die für Microsoft Edge gelten
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571827"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="69bdf-102">Erweiterte Authentifizierungskonzepte, die für Microsoft Edge gelten</span><span class="sxs-lookup"><span data-stu-id="69bdf-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="69bdf-103">Im folgenden sind die erweiterten Authentifizierungskonzepte aufgeführt, die auf Microsoft Edge zutreffen:</span><span class="sxs-lookup"><span data-stu-id="69bdf-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="69bdf-104">**Proaktive Authentifizierung**</span><span class="sxs-lookup"><span data-stu-id="69bdf-104">**Proactive Authentication**</span></span>

<span data-ttu-id="69bdf-105">Wenn Sie die [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -Richtlinie aktivieren, versucht Microsoft Edge die aktive Authentifizierung von angemeldeten Benutzern über Microsoft-Dienste.</span><span class="sxs-lookup"><span data-stu-id="69bdf-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="69bdf-106">In regelmäßigen Abständen wird ein Onlinedienst verwendet, um nach einem aktualisierten Manifest zu suchen, das die Konfiguration für die proaktive Authentifizierung enthält.</span><span class="sxs-lookup"><span data-stu-id="69bdf-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="69bdf-107">Vorteile: die proaktive Authentifizierung ermöglicht die Authentifizierung für wichtige Dienste, wie beispielsweise die Registerkarte "Office New".</span><span class="sxs-lookup"><span data-stu-id="69bdf-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="69bdf-108">Wenn Bing als Such Modul verwendet wird, verbessert die proaktive Authentifizierung auch die Leistung der Adressleiste und hilft bei der Generierung von Suchergebnissen, die auf die Anforderungen Ihres Unternehmens zugeschnitten sind.</span><span class="sxs-lookup"><span data-stu-id="69bdf-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="69bdf-109">**Windows Hello CredUI für die NTLM-Authentifizierung**</span><span class="sxs-lookup"><span data-stu-id="69bdf-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="69bdf-110">Wenn einmaliges Anmelden (Single Sign-on, SSO) nicht verfügbar ist, wenn eine Website versucht, sich über den NTLM-oder Negotiate-Mechanismus am Benutzer anzumelden, ermöglicht diese Funktion dem Benutzer, die Betriebssystem Anmeldeinformationen für die Website freizugeben und die Authentifizierungsanforderung mithilfe der Windows Hello cred-Benutzeroberfläche zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="69bdf-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="69bdf-111">Dieser Anmelde Fluss wird nur in Windows 10 und nur für Benutzer angezeigt, die nicht SSO während einer NTLM-oder Negotiate-Herausforderung erhalten.</span><span class="sxs-lookup"><span data-stu-id="69bdf-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="69bdf-112">**Automatisches Anmelden mit gespeicherten Kennwörtern**</span><span class="sxs-lookup"><span data-stu-id="69bdf-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="69bdf-113">Benutzer, die Kennwörter in Microsoft Edge speichern, können die automatische Anmeldung bei Websites aktivieren, auf denen Sie Anmeldeinformationen gespeichert haben.</span><span class="sxs-lookup"><span data-stu-id="69bdf-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="69bdf-114">Benutzer können diese Funktion in Edge://Settings/passwords aktivieren oder deaktivieren, und Sie können Sie in den [Password Manager-](https://go.microsoft.com/fwlink/?linkid=2134622) Richtlinien konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="69bdf-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
