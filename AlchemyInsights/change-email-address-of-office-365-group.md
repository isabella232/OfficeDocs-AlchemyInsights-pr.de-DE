---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733686"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe

Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern. Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.

Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Beispiel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
