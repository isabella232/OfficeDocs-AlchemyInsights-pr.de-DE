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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="45329-102">Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="45329-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="45329-103">Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern.</span><span class="sxs-lookup"><span data-stu-id="45329-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="45329-104">Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.</span><span class="sxs-lookup"><span data-stu-id="45329-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="45329-105">Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:</span><span class="sxs-lookup"><span data-stu-id="45329-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="45329-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="45329-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="45329-107">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="45329-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
