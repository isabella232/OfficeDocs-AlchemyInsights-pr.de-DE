---
title: Verwalten eines synchronisierten Benutzers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541988"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Primäre e-Mail-Adresse kann nicht festgelegt oder Benutzerattribute geändert werden

Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer-oder Objektattribute nicht mithilfe des Microsoft 365 Admin Center geändert werden.

Verwenden Sie zum vollständigen verwalten synchronisierter Benutzer und aller Attribute Ihre lokale Active Directory-Benutzer-und Gruppen Verwaltungskonsole (AdsiEdit. msc).  

Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in den folgenden allgemeinen Beispielen gezeigt: 
- Gruppe-MsolUser-userPrincipalName User@yourdomain.onmicrosoft.com-AlternateEmailAddresses User2@yourvanitydomain.onmicrosoft.com
- Sets-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com"-DisplayName "Test User"-Nachname "User"-Titel "Manager"-Abteilung "HR"
- Remove-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com