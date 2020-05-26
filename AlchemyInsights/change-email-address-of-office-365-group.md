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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282350"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="29855-102">Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="29855-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="29855-103">Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe über das Admin Center ändern.</span><span class="sxs-lookup"><span data-stu-id="29855-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="29855-104">Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.</span><span class="sxs-lookup"><span data-stu-id="29855-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="29855-105">Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe zu ändern:</span><span class="sxs-lookup"><span data-stu-id="29855-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="29855-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="29855-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="29855-107">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="29855-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
