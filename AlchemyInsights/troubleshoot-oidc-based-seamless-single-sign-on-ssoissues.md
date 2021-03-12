---
title: Behandeln von Problemen mit dem OIDC-basierten einmaligen Anmelden (Single Sign-On, SSO)
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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726922"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Behandeln von Problemen mit dem OIDC-basierten einmaligen Anmelden (Single Sign-On, SSO)

- Informationen zum Hinzufügen einer OIDC-basierten App zu Ihrem Azure-Mandanten finden Sie unter Schnellstart: Einrichten des OIDC-basierten einmaligen Anmeldens [(Single Sign-On, SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten.
- Weitere Informationen zu Apps, die den OpenID Connect-Standard verwenden, um einmaliges Anmelden zu implementieren, finden Sie unter [Understand OIDC-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Informationen für den Fall, dass Sie Ihren Code schreiben möchten, indem Sie direkt HTTP-Anforderungen senden und verarbeiten oder eine Open-Source-Bibliothek eines Drittanbieters verwenden, anstatt eine unserer Open-Source-Bibliotheken zu verwenden, finden Sie unter [OAuth 2.0-](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)und OpenID Connect-Protokolle auf der Microsoft Identity Platform .

**Protokolle**

1. [Microsoft-Identitätsplattform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) und impliziter Erteilungsfluss – Das definierende Merkmal der impliziten Gewährung ist, dass Token (ID-Token oder Zugriffstoken) direkt vom /authorize-Endpunkt anstelle des /token-Endpunkts zurückgegeben werden. Dies wird häufig als Teil des Autorisierungscodeflusses verwendet, in dem so genannten **"Hybridfluss" –** abrufen des ID-Tokens für die /authorize-Anforderung zusammen mit einem Autorisierungscode . In diesem Artikel wird beschrieben, wie Sie direkt für das Protokoll in Ihrer Anwendung Programmieren, um Token von Azure AD an fordern.
2. [Microsoft Identity Platform und OAuth 2.0-Autorisierungscodefluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Die OAuth 2.0-Autorisierungscode-Erteilung kann in Apps verwendet werden, die auf einem Gerät installiert sind, um Zugriff auf geschützte Ressourcen wie Web-APIs zu erhalten. Mithilfe der Microsoft Identity Platform-Implementierung von OAuth 2.0 können Sie Anmelde- und API-Zugriff auf Ihre mobilen Apps und **Desktop-Apps hinzufügen.** In diesem Artikel wird beschrieben, wie Sie direkt mit dem Protokoll in Ihrer Anwendung mithilfe einer beliebigen Sprache programmieren.
3. [Microsoft Identity Platform und OpenID Connect-Protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) : Wenn Sie die Implementierung von OpenID Connect der Microsoft Identity Platform verwenden, können Sie Ihren Apps Anmelde- und API-Zugriff hinzufügen. Dieser Artikel zeigt, wie Sie dies unabhängig von der Sprache tun können, und beschreibt, wie Sie HTTP-Nachrichten senden und empfangen, ohne **Open-Source-Bibliotheken** von Microsoft zu verwenden.
4. [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – You can use the OAuth 2.0 client credentials grant specified in RFC 6749, sometimes called **two-legged OAuth**, to access web-hosted resources by using the identity of an application. Diese Art der Gewährung wird häufig für Server-zu-Server-Interaktionen verwendet, die im Hintergrund ausgeführt werden müssen, ohne dass eine direkte Interaktion mit einem Benutzer erforderlich ist. Diese Arten von Anwendungen werden häufig als **Daemons oder** **Dienstkonten bezeichnet.** In diesem Artikel wird beschrieben, wie Sie direkt für das Protokoll in Ihrer Anwendung programmieren.
