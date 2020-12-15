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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416695"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="1fac8-102">Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="1fac8-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="1fac8-103">Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern.</span><span class="sxs-lookup"><span data-stu-id="1fac8-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="1fac8-104">Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.</span><span class="sxs-lookup"><span data-stu-id="1fac8-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="1fac8-105">Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:</span><span class="sxs-lookup"><span data-stu-id="1fac8-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="1fac8-106">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="1fac8-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
