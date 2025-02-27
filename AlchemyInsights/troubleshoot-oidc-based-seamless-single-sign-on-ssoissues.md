---
title: Behandeln von OIDC-basierten Problemen mit einmaligem Anmelden (Seamless Single Sign-On, SSO)
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
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105777"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Behandeln von OIDC-basierten Problemen mit einmaligem Anmelden (Seamless Single Sign-On, SSO)

- Weitere Informationen zum Hinzufügen einer OIDC-basierten App zu Ihrem Azure-Mandanten finden Sie unter [Schnellstart: Einrichten des OIDC-basierten einmaligen Anmeldens (Single Sign-On, SSO) für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Weitere Informationen zu Apps, die den OpenID-Verbinden-Standard zum Implementieren von Single Sign-On verwenden, finden Sie unter ["Grundlegendes zu OIDC-basiertem einmaligem Anmelden".](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Informationen für den Fall, dass Sie Ihren Code schreiben möchten, indem Sie HTTP-Anforderungen direkt senden und verarbeiten oder eine Open-Source-Bibliothek eines Drittanbieters verwenden, anstatt eine unserer Open-Source-Bibliotheken zu verwenden, finden Sie unter [OAuth 2.0 und OpenID Verbinden Protokolle auf der Microsoft Identity Platform.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)

**Protokolle**

1. [Microsoft Identity Platform und impliziter Genehmigungsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – Das definierende Merkmal der impliziten Genehmigung ist, dass Token (ID-Token oder Zugriffstoken) direkt vom /authorize-Endpunkt anstelle des /token-Endpunkts zurückgegeben werden. Dies wird häufig als Teil des Autorisierungscodeflusses verwendet, in dem so genannten **"Hybridfluss" – abrufen des ID-Tokens in der /authorize-Anforderung zusammen mit einem Autorisierungscode.** In diesem Artikel wird beschrieben, wie Sie direkt für das Protokoll in Ihrer Anwendung programmieren, um Token von Azure AD anzufordern.
2. [Microsoft Identity Platform und OAuth 2.0-Autorisierungscodefluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Die OAuth 2.0-Autorisierungscodegenehmigung kann in Apps verwendet werden, die auf einem Gerät installiert sind, um Zugriff auf geschützte Ressourcen wie Web-APIs zu erhalten. Mithilfe der Microsoft Identity Platform Implementierung von OAuth 2.0 können Sie **Ihren mobilen und Desktop-Apps Anmelde- und API-Zugriff hinzufügen.** In diesem Artikel wird beschrieben, wie Sie mithilfe einer beliebigen Sprache direkt mit dem Protokoll in Ihrer Anwendung programmieren.
3. [Microsoft Identity Platform und das OpenID Verbinden-Protokoll:](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) Wenn Sie die Implementierung von OpenID Verbinden durch die Microsoft Identity Platform verwenden, können Sie Ihren Apps Anmelde- und API-Zugriff hinzufügen. In diesem Artikel wird beschrieben, wie dies unabhängig von der Sprache funktioniert, und es wird beschrieben, wie **HTTP-Nachrichten gesendet und empfangen werden, ohne Microsoft-Open-Source-Bibliotheken** zu verwenden.
4. [Microsoft Identity Platform und dem OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Sie können die in RFC 6749 angegebene OAuth 2.0-Clientanmeldeinformationsgewährung verwenden, die manchmal als **zwei legged OAuth** bezeichnet wird, um mithilfe der Identität einer Anwendung auf webgehostete Ressourcen zuzugreifen. Diese Art der Erteilung wird häufig für Server-zu-Server-Interaktionen verwendet, die im Hintergrund ohne sofortige Interaktion mit einem Benutzer ausgeführt werden müssen. Diese Arten von Anwendungen werden häufig als **Daemons** oder **Dienstkonten** bezeichnet. In diesem Artikel wird beschrieben, wie Sie direkt mit dem Protokoll in Ihrer Anwendung programmieren.
