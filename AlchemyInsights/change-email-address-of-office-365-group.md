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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="4098f-102">Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="4098f-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="4098f-103">Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern.</span><span class="sxs-lookup"><span data-stu-id="4098f-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="4098f-104">Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.</span><span class="sxs-lookup"><span data-stu-id="4098f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="4098f-105">Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:</span><span class="sxs-lookup"><span data-stu-id="4098f-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="4098f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="4098f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="4098f-107">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="4098f-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
