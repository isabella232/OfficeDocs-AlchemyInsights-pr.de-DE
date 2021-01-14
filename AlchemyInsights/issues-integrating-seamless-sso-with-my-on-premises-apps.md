---
title: Probleme bei der Integration des nahtlosen einmaligen Einmaliges Nutzens in meine lokalen Apps
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848773"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Probleme bei der Integration des nahtlosen einmaligen Einmaliges Nutzens in meine lokalen Apps

Gehen Sie wie folgt vor, um Probleme bei der Integration von nahtloser einmaliger Anmeldung in lokale Anwendungen zu beheben:

**Empfohlene Schritte**

1. Informationen zum Konfigurieren einer  **lokalen** Anwendung für einmaliges Anmelden über Anwendungsproxy finden Sie unter Kennworttresor für einmaliges Anmelden [mit Anwendungsproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Behandlung von Anwendungsproxyproblemen:** Es wird empfohlen, dass Sie mit der Überprüfung des Problembehandlungsflusses, des Debuggens von Problemen mit dem Anwendungsproxyconnector beginnen, um festzustellen, ob Anwendungsproxyconnectors ordnungsgemäß konfiguriert sind. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) Wenn sie weiterhin Probleme beim Herstellen einer Verbindung mit der Anwendung haben, führen Sie die Schritte zur Problembehandlung unter Debuggen von [Anwendungsproxyanwendungsproblemen aus.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Sie können [CORS-Probleme mithilfe](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) der folgenden Browserdebuggertools identifizieren:
    1. Starten Sie den Browser, und navigieren Sie zur Web-App.
    1. Drücken **Sie F12,** um die Debugkonsole zu starten.
    1. Versuchen Sie, die Transaktion zu reproduzieren, und überprüfen Sie die Konsolenmeldung. Eine CORS-Verletzung erzeugt einen Konsolenfehler über den Ursprung.
    1. Einige CORS-Probleme können nicht behoben werden, z. B. wenn Ihre App zur Authentifizierung login.microsoftonline.com und das Zugriffstoken abläuft. Der CORS-Aufruf schlägt dann fehl. Eine Problemumgehung für dieses Szenario besteht in der Verlängerung der Lebensdauer des Zugriffstokens, um zu verhindern, dass es während der Sitzung eines Benutzers ab läuft. Weitere Informationen hierzu finden Sie unter ["Konfigurierbare Tokenlebensdauern" in Microsoft Identity Platform.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Empfohlene Dokumente**

- [Konfigurieren des einmaligen Anmeldens bei einer Anwendungsproxyanwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Einmaliges Anmelden von SAML für lokale Anwendungen mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Verstehen und Lösen von Azure Active Directory-Anwendungsproxy-CORS-Problemen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Problembehandlung für Konfigurationen mit eingeschränkter Kerberos-Delegierung für Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)