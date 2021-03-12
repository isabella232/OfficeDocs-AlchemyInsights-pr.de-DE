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
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Problembehandlung bei Problemen mit kennwortbasiertem nahtlosen einmaligen Anmelden (Single Sign-On, SSO)

Informationen zu den Grundlagen des kennwortbasierten SSO finden Sie unter [Kennwortbasierte Authentifizierung mit Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurieren von kennwortbasiertem SSO**

1. [Konfigurieren des kennwortbasierten einmaligen Anmeldens](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – In diesem Artikel wird die kennwortbasierte SSO-Option ausführlicher behandelt. Wenn für die Anwendung, die Sie hinzufügen, eine benutzerdefinierte Konfiguration erforderlich ist und Sie kennwortbasiertes SSO verwenden müssen, ist dieser Artikel für Sie da.
2. [Konfigurieren der kennwortbasierten einmaligen Anmeldung für On-Prem-Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Anwendungsproxy unterstützt mehrere Modi für einmaliges Anmelden. Die kennwortbasierte Anmeldung ist für Anwendungen vorgesehen, die eine Kombination aus Benutzername und Kennwort für die Authentifizierung verwenden. Wenn Sie die kennwortbasierte Anmeldung für Ihre Anwendung konfigurieren, müssen sich Ihre Benutzer einmal bei der lokalen Anwendung anmelden. Danach speichert Azure Active Directory die Anmeldeinformationen und stellt sie automatisch der Anwendung bereit, wenn Ihre Benutzer remote darauf zugreifen.
    - Sie sollten Ihre App bereits mit Anwendungsproxy veröffentlicht und getestet haben. Wenn nicht, führen Sie die Schritte unter Veröffentlichen von Anwendungen mithilfe des [Azure AD-Anwendungsproxys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) aus, und setzen Sie dann Ihre Konfiguration von kennwortbasiertem SSO für vorab installierte Apps fort.

Informationen zur Problembehandlung bei kennwortbasiertem SSO finden Sie unter Problembehandlung für [kennwortbasierte einmaliges](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) Anmelden in Azure AD.
