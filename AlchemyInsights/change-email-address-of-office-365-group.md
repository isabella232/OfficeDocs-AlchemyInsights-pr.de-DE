---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580656"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe

Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern. Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.

Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Beispiel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
