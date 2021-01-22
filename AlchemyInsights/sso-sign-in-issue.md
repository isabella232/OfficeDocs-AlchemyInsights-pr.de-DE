---
title: Nahtlose SSO-Benutzer-Anmeldeprobleme
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919202"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Nahtlose SSO-Benutzer-Anmeldeprobleme

Nachdem der Benutzer authentifiziert wurde, speichert der Browser die Anmeldeinformationen des Benutzers zwischen, sodass sich die Anwendung im selben Browser automatisch mit demselben Konto anmeldet. Dies kann es für einen anderen Benutzer oder einen einzelnen Benutzer schwierig machen, sich bei mehreren Konten auf einem Gerät zu anmelden. Lösung: 1. Versuchen Sie, sich in einem anderen Browser zu anmelden. 2. Löschen Sie den Cache des Browsers und/oder Cookies, und versuchen Sie es erneut.

Wenn weiterhin Anmeldeprobleme auftreten, empfehlen wir Folgendes, um die Lösungsschritte zu diagnostizieren und zu automatisieren:

1. Installieren Sie [die "My Apps Secure Browser Extension",](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) um Azure Active Directory (Azure AD) bei der Bereitstellung besserer Diagnosen und Lösungen zu unterstützen, wenn Sie die Testerfahrung im Azure-Portal verwenden.
2. Reproduzieren Sie den Fehler mithilfe der Testerfahrung auf der Seite "App-Konfiguration" im Azure-Portal. Weitere Informationen finden Sie unter [Debuggen von SAML-basierten Anwendungen für einmaliges Anmelden.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Wenn Sie die Testerfahrung im Azure-Portal mit der Sicheren Browsererweiterung "Meine Apps" verwenden, können Sie **Schritt 4 überspringen.**
4. So öffnen Sie die SAML-basierte Konfigurationsseite für einmaliges Anmelden:
    - Öffnen Sie [das Azure-Portal,](https://portal.azure.com/) und melden Sie sich als **globaler Administrator oder** **Coadmin an.**
    - Öffnen Sie die Azure  **Active Directory-Erweiterung,** indem Sie oben im linken Hauptnavigationsmenü alle Dienste auswählen.
    - Geben Sie "Azure Active Directory" in das Filtersuchfeld ein, und wählen Sie das **Azure Active Directory-Element** aus.
    - Wählen Sie im linken **Navigationsmenü** von Azure Active Directory die Option "Enterprise-Anwendungen" aus.
    - Wählen **Sie "Alle Anwendungen"** aus, um eine Liste aller Anwendungen anzeigen zu können. Wenn die Anwendung, die Sie hier anzeigen möchten, nicht angezeigt wird, verwenden Sie  das Steuerelement **"Filter"** oben in der Liste "Alle Anwendungen",  und legen Sie die Option "Anzeigen" auf **"Alle Anwendungen" festgelegt.**
    - Wählen Sie die Anwendung aus, die Sie für einmaliges Anmelden konfigurieren möchten.
    - Nachdem die Anwendung geladen wurde, **wählen** Sie im linken Navigationsmenü der Anwendung die Option "Einmaliges Anmelden" aus.
    - Wählen **Sie SAML-basiertes SSO aus.**
5. Weitere Informationen zu den empfohlenen Schritten finden Sie basierend auf dem Fehler unter "Probleme beim Anmelden bei saml-basierten, für einmaliges Anmelden [konfigurierten Apps".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Informationen zur Problembehandlung bei anderen Problemen mit der Benutzer anmeldung finden Sie in den folgenden Anleitungen:
    - [Single-Sign-On-SAML-Protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [How to: Troubleshoot sign-in errors using Azure Active Directory reports](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Unerwartete Zustimmungsaufforderung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Fehler bei der Zustimmung des Benutzers](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Probleme beim Anmelden von "Meine Apps"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Fehler auf der Anmeldeseite der Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem beim Anmelden bei einer Microsoft App](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
