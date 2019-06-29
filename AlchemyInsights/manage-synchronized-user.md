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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380504"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Primäre e-Mail-Adresse kann nicht festgelegt oder Benutzerattribute geändert werden

Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer-oder Objektattribute nicht mithilfe des Admin Centers geändert werden.
Verwenden Sie zum vollständigen verwalten synchronisierter Benutzer und aller Attribute Ihre lokale Active Directory-Benutzer-und Gruppen Verwaltungskonsole (AdsiEdit. msc).  

Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in den folgenden allgemeinen Beispielen gezeigt: 
- Gruppe-MsolUser-userPrincipalName User@yourdomain.onmicrosoft.com-AlternateEmailAddresses User2@yourvanitydomain.onmicrosoft.com
- Sets-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com"-DisplayName "Test User"-Nachname "User"-Titel "Manager"-Abteilung "HR"
- Remove-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com