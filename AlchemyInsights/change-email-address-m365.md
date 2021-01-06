---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756556"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="2a549-102">Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2a549-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="2a549-103">Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams über das [Microsoft 365 Admin Center](https://admin.microsoft.com/) ändern.</span><span class="sxs-lookup"><span data-stu-id="2a549-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="2a549-104">Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.</span><span class="sxs-lookup"><span data-stu-id="2a549-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="2a549-105">Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe bzw. von Teams zu ändern:</span><span class="sxs-lookup"><span data-stu-id="2a549-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="2a549-106">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="2a549-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
