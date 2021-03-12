---
title: Problembehandlung bei Problemen mit kennwortbasiertem nahtlosen einmaligen Anmelden (Single Sign-On, SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709496"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="6beca-102">Problembehandlung bei Problemen mit kennwortbasiertem nahtlosen einmaligen Anmelden (Single Sign-On, SSO)</span><span class="sxs-lookup"><span data-stu-id="6beca-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="6beca-103">Informationen zu den Grundlagen des kennwortbasierten SSO finden Sie unter [Kennwortbasierte Authentifizierung mit Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="6beca-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="6beca-104">**Konfigurieren von kennwortbasiertem SSO**</span><span class="sxs-lookup"><span data-stu-id="6beca-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="6beca-105">[Konfigurieren des kennwortbasierten einmaligen Anmeldens](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – In diesem Artikel wird die kennwortbasierte SSO-Option ausführlicher behandelt.</span><span class="sxs-lookup"><span data-stu-id="6beca-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="6beca-106">Wenn für die Anwendung, die Sie hinzufügen, eine benutzerdefinierte Konfiguration erforderlich ist und Sie kennwortbasiertes SSO verwenden müssen, ist dieser Artikel für Sie da.</span><span class="sxs-lookup"><span data-stu-id="6beca-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="6beca-107">[Konfigurieren der kennwortbasierten einmaligen Anmeldung für On-Prem-Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Anwendungsproxy unterstützt mehrere Modi für einmaliges Anmelden.</span><span class="sxs-lookup"><span data-stu-id="6beca-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="6beca-108">Die kennwortbasierte Anmeldung ist für Anwendungen vorgesehen, die eine Kombination aus Benutzername und Kennwort für die Authentifizierung verwenden.</span><span class="sxs-lookup"><span data-stu-id="6beca-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="6beca-109">Wenn Sie die kennwortbasierte Anmeldung für Ihre Anwendung konfigurieren, müssen sich Ihre Benutzer einmal bei der lokalen Anwendung anmelden.</span><span class="sxs-lookup"><span data-stu-id="6beca-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="6beca-110">Danach speichert Azure Active Directory die Anmeldeinformationen und stellt sie automatisch der Anwendung bereit, wenn Ihre Benutzer remote darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="6beca-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="6beca-111">Sie sollten Ihre App bereits mit Anwendungsproxy veröffentlicht und getestet haben.</span><span class="sxs-lookup"><span data-stu-id="6beca-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="6beca-112">Wenn nicht, führen Sie die Schritte unter Veröffentlichen von Anwendungen mithilfe des [Azure AD-Anwendungsproxys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) aus, und setzen Sie dann Ihre Konfiguration von kennwortbasiertem SSO für vorab installierte Apps fort.</span><span class="sxs-lookup"><span data-stu-id="6beca-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="6beca-113">Informationen zur Problembehandlung bei kennwortbasiertem SSO finden Sie unter Problembehandlung für [kennwortbasierte einmaliges](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) Anmelden in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6beca-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
