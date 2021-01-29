---
title: Konfigurieren und Anpassen von Anwendungen
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50043982"
---
# <a name="configure-and-customize-applications"></a>Konfigurieren und Anpassen von Anwendungen

**Konfigurieren von Anwendungen**

1. Schnellstart: Das Konfigurieren von Eigenschaften für eine Anwendung in Ihrem [Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) zeigt Ihnen, wie Sie einige der Eigenschaften für eine App konfigurieren.
2. Um Ihre Anwendungen in Azure Active Directory [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) zu integrieren, haben wir eine Sammlung von Lernprogrammen entwickelt, die Sie durch die Konfiguration unterstützen.
3. [Die Konfiguration einer Anwendungsproxyanwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) hilft Ihnen zu verstehen, wie Sie eine Anwendungsproxyanwendung in Azure AD konfigurieren, um Ihre lokalen Anwendungen in der Cloud verfügbar zu machen.
4. [Laden Sie PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)herunter, und konfigurieren Sie Ihre Anwendung: Befolgen Sie die Anweisungen unter *"PingAccess* für Azure AD konfigurieren", um Anwendungen zu schützen, die mit Dem Microsoft Azure AD-Anwendungsproxy auf der Website für PingIdentität veröffentlicht wurden, und laden Sie die neueste Version von PingAccess herunter.

**Fehler bei falsch konfigurierter Anwendung (AADSTS650056)**

1. Stellen Sie sicher, dass Sie über die vom Anwendungsbesitzer bereitgestellte Anmeldeadresse auf die Anwendung zugreifen. Andernfalls sollten Sie sich über den normalen Prozess bei der Anwendung anmelden. In den meisten Fällen wird dies automatisch aufgelöst. Wenn dies nicht der Fehler ist, kann dieser Beitrag bei der Problembehandlung und Lösung helfen.
2. **Wenn Ihre Organisation die Anwendung besitzt** (d. h. die Anwendungsregistrierung befindet sich in Ihrer Organisation):
    - Wir empfehlen mindestens, dass die `User.Read` oder die delegierte Berechtigung von Microsoft `openid` **Graph** hinzugefügt wird.
    - Stellen Sie sicher, dass die Anwendung und alle ihre Berechtigungen zustimmen. Sie können dies überprüfen, indem Sie die Spalte **"Status"** der Anwendungsregistrierung in den **API-Berechtigungen anzeigen.**
    - In einigen Szenarien ist die Anwendung möglicherweise ein Drittanbieter, sie kann jedoch in Ihrer Organisation registriert sein. Bestätigen Sie, ob diese Anwendung in Ihren App-Registrierungen (keine Enterprise-Anwendungen) aufgeführt ist.
    - Wenn diese Fehlermeldung weiterhin angezeigt wird. Anschließend müssen Sie möglicherweise die in Schritt 4 beschriebene Zustimmungs-URL **erstellen.**
3. **Wenn Ihre Organisation nicht der Anwendungsbesitzer ist und sie als Drittanbieteranwendung verwendet:**
    - Wenn Sie der Globale/Unternehmensadministrator sind, sollte der Zustimmungsbildschirm angezeigt werden. Stellen Sie sicher, dass Sie das Kontrollkästchen **"Zustimmung im Namen Ihrer Organisation" aktivieren.**
    - Wenn der Zustimmungsbildschirm nicht angezeigt wird, löschen Sie die Enterprise-Anwendung, und versuchen Sie es erneut.
    - Wenn diese Fehlermeldung weiterhin angezeigt wird. Anschließend müssen Sie möglicherweise die in Schritt 4 beschriebene Zustimmungs-URL **erstellen.**
4. Erstellen Sie die zu verwendende **Zustimmungs-URL** manuell: Wenn die Anwendung für den Zugriff auf eine bestimmte Ressource konzipiert ist, können Sie möglicherweise nicht die Zustimmungsschaltflächen aus dem Azure-Portal verwenden. Sie müssen ihre eigene Zustimmungs-URL manuell generieren und diese verwenden.
    - Sie müssen das und das vom `{App-Id}` `{App-Uri-Id}` Anwendungsbesitzer erhalten. `{Tenant-Id}` wird Ihre Mandanten-ID sein. Dies ist entweder `yourdomain.onmicrosoft.com` Ihre Verzeichnis-ID.
    - Wenn die Anwendung für die Ressource auf sich selbst zu zugegriffen hat, ist dies der `{App-Id}` `{App-Uri-Id}` gleiche.
5. Weitere Informationen finden Sie unter ["Probleme beim Anmelden bei SAML-basierten apps für einmaliges Anmelden".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Anpassen von Anwendungen**

- Hinzufügen von Branding zur [Azure Active Directory-Anmeldeseite](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) Ihrer Organisation – Verwenden Sie das Logo Ihrer Organisation und benutzerdefinierte Farbschemas, um Ihren Azure Active Directory (Azure AD)-Anmeldeseiten ein einheitliches Aussehen und Gefühl zu bieten.
- [Fügen Sie Ihren benutzerdefinierten Domänennamen mithilfe des Azure Active Directory-Portals hinzu–](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) Jeder neue Azure AD-Mandant verfügt über einen anfänglichen Domänennamen. Sie können den ursprünglichen Domänennamen nicht ändern oder löschen, aber Sie können die Namen Ihrer Organisation hinzufügen. Das Hinzufügen von benutzerdefinierten Domänennamen hilft Ihnen beim Erstellen von Benutzernamen, die Ihren Benutzern vertraut sind.
