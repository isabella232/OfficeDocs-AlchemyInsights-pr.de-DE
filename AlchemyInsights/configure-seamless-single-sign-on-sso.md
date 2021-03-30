---
title: Konfigurieren des nahtlosen einmaligen Anmeldens (Single Sign-On, SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402266"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurieren des nahtlosen einmaligen Anmeldens (Single Sign-On, SSO)

**Konfigurieren von Anwendungen**

1. Sie sollten die Werte vom Anwendungsanbieter erhalten. Sie können die Werte manuell eingeben oder eine Metadatendatei hochladen, um den Wert der Felder zu extrahieren.
2. Viele Apps wurden bereits für die Verwendung mit Azure AD vorkonfiguriert. Diese Apps sind im Katalog der Apps aufgeführt, die Sie durchsuchen können, wenn Sie Ihrem Azure AD-Mandanten eine App hinzufügen. Die [Schnellstartreihe führt](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) Sie durch den Prozess.
3. Um eine Nicht-Kataloganwendung zu erstellen, können Sie auf **+ Eigene** Anwendungsschaltfläche erstellen klicken und Ihrer Anwendung einen Namen geben.
    - Standardmäßig wird jede andere Anwendung integrieren ausgewählt, die Sie nicht **im** Katalog finden, was die richtige Option für Nicht-Katalog-Anwendungen ist.
    - Sobald Sie **nach** dem Eingeben des Namens für die Anwendung auf Erstellen getroffen haben, wird eine neue Nicht-Katalog-Enterprise-Anwendung erstellt.
    - Anschließend können Sie zu **Einmaliges Anmelden** unter **Verwalten** dieser Anwendung navigieren, und Sie können verschiedene Techniken für die Implementierung in Ihrer Umgebung sehen.

**Konfigurieren von nahtloser SSO für eine bestimmte Anwendung**

Für die Apps im Katalog finden Sie ausführliche, schrittweise Anweisungen. Um auf die Schritte zu zugreifen, können Sie eine Liste aller App-Konfigurationstutorial unter [SaaS-App-Konfigurations-Tutorials durchsuchen.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurieren von SAML-basiertem SSO**

1. [Schnellstart: Einrichten von SAML-basierten einmaligen Anmeldungen (Single Sign-On, SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten .
2. Weitere Informationen zur SAML-basierten Option für einmaliges Anmelden finden Sie unter [Understand SAML-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Informationen zu den SAML 2.0-Authentifizierungsanforderungen und -antworten, die Azure Active Directory (Azure AD) für einmaliges Sign-On (Single Sign-On, SSO) unterstützt, finden Sie unter [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Informationen zum Erstellen und Konfigurieren eines SAML-basierten einmaligen Anmeldens (SSO) für Ihre Anwendung in Azure Active Directory (Azure AD) mithilfe der Microsoft Graph-API finden Sie unter [Configure SAML-based single sign-on for your application using the Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Informationen dazu, wie Azure AD das SAML-Protokoll verwendet, finden Sie unter [How the Microsoft identity platform uses the SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurieren von Token und Ansprüchen**

1. [How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Informationen zum Konfigurieren von Ansprüchen mithilfe von PowerShell finden Sie unter [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Informationen zum Konfigurieren optionaler Ansprüche finden Sie unter [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Informationen zur Verwendung von Verzeichnisschemaerweiterungsattributen zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen finden Sie unter [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Informationen zum Konfigurieren von Tokenlebensdauern finden Sie unter [Configurable token lifetimes in the Microsoft identity platform (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfigurieren von Tokenlebensdauerrichtlinien (Vorschau)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – In diesem Artikel wird ein allgemeines Richtlinienszenario beschrieben, mit dem Sie neue Regeln für die Tokenlebensdauer durchsetzen können. Im Beispiel erfahren Sie, wie Sie eine Richtlinie erstellen, für die Benutzer sich häufiger in Ihrer Web-App authentifizieren müssen.

**Problembehandlung bei der SSO-Konfiguration**

- Häufig gestellte Fragen zu Azure Active Directory Seamless Single Sign-On (Seamless SSO) finden Sie unter [Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informationen zur Problembehandlung zu häufigen Problemen im Zusammenhang mit Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO) finden Sie unter [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
