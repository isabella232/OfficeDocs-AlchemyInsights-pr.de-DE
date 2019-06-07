---
title: Einrichten von DKIM in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765077"
---
# <a name="setup-dkim-in-office-365"></a>Einrichten von DKIM in Office 365

Die vollständigen Anweisungen zum Konfigurieren von DKIM für benutzerdefinierte Domänen in Office 365 finden Sie [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Für **jede** benutzerdefinierte Domäne müssen Sie **zwei** DKIM-CNAME-Einträge im DNS-Hostingdienst Ihrer Domäne erstellen (in der Regel die Domänenregistrierungsstelle). Für contoso.com und fourthcoffee.com sind beispielsweise vier DKIM-CNAME-Einträge erforderlich: zwei für contoso.com und zwei für fourthcoffee.com.

   Die DKIM-CNAME-Einträge für **jede** benutzerdefinierte Domäne verwenden die folgenden Formate:

   - **Hostname**:`selector1._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostname**:`selector2._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> ist der Text Links `.mail.protection.outlook.com` neben dem angepassten MX-Eintrag für die benutzerdefinierte Domäne (beispielsweise `contoso-com` für die Domäne contoso.com). \<InitialDomain\> ist die Domäne, die Sie bei der Registrierung für Office 365 verwendet haben (beispielsweise contoso.onmicrosoft.com).

2. Nachdem Sie die CNAME-Einträge für Ihre benutzerdefinierten Domänen erstellt haben, führen Sie die folgenden Schritte aus:

   a. [Melden Sie sich bei Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) mit Ihrem Firmen- oder Schulkonto an.

   b. Klicken Sie oben links auf das App-Startsymbol, und wählen Sie **Admin** aus.

   c. Erweitern Sie im unteren linken Navigationsbereich **Admin**, und klicken Sie dann auf **Exchange**.

   d. Wechseln Sie zu **Protection** > **DKIM**.

   e. Wählen Sie die Domäne aus, und wählen Sie dann für **Signieren Nachrichten für diese Domäne mit DKIM-Signaturen** **aktivieren** aus. Wiederholen Sie diesen Schritt für jede benutzerdefinierte Domäne.
