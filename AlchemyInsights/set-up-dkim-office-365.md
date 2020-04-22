---
title: Setup-DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645671"
---
# <a name="setup-dkim"></a>Setup-DKIM

Die vollständigen Anweisungen zum Konfigurieren von DKIM für benutzerdefinierte Domänen in Microsoft 365 finden Sie [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Für **jede** benutzerdefinierte Domäne müssen Sie **zwei** DKIM-CNAME-Einträge im DNS-Hostingdienst Ihrer Domäne erstellen (in der Regel die Domänenregistrierungsstelle). Für contoso.com und fourthcoffee.com sind beispielsweise vier DKIM-CNAME-Einträge erforderlich: zwei für contoso.com und zwei für fourthcoffee.com.

   Die DKIM-CNAME-Einträge für **jede** benutzerdefinierte Domäne verwenden die folgenden Formate:

   - **Hostname**:`selector1._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostname**:`selector2._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> ist der Text Links `.mail.protection.outlook.com` neben dem angepassten MX-Eintrag für die benutzerdefinierte Domäne (beispielsweise `contoso-com` für die Domäne contoso.com). \<InitialDomain\> ist die Domäne, die Sie bei der Registrierung bei Microsoft 365 verwendet haben (beispielsweise contoso.onmicrosoft.com).

2. Nachdem Sie die CNAME-Einträge für Ihre benutzerdefinierten Domänen erstellt haben, führen Sie die folgenden Schritte aus:

   a. [melden Sie sich bei Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) mit ihrem geschäftlichen oder Schulkonto an.

   b. Klicken Sie oben links auf das App-Startsymbol, und wählen Sie **Admin** aus.

   c. Erweitern Sie im unteren linken Navigationsbereich **Admin**, und klicken Sie dann auf **Exchange**.

   d. Wechseln Sie zu **Protection** > **DKIM**.

   e. Wählen Sie die Domäne aus, und wählen Sie dann für **Signieren Nachrichten für diese Domäne mit DKIM-Signaturen** **aktivieren** aus. Wiederholen Sie diesen Schritt für jede benutzerdefinierte Domäne.
