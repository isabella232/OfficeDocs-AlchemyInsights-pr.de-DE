---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819043"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="3b711-102">Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="3b711-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="3b711-103">Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern.</span><span class="sxs-lookup"><span data-stu-id="3b711-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="3b711-104">Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.</span><span class="sxs-lookup"><span data-stu-id="3b711-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="3b711-105">Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:</span><span class="sxs-lookup"><span data-stu-id="3b711-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="3b711-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="3b711-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="3b711-107">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="3b711-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
