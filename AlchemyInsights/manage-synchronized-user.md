---
title: Verwalten eines synchronisierten Benutzers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777676"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="6ee97-102">Primäre e-Mail-Adresse kann nicht festgelegt, Benutzerattribute geändert oder ein synchronisierter Benutzer entfernt/gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="6ee97-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="6ee97-103">Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer-oder Objektattribute nicht mithilfe des Microsoft 365 Admin Center geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6ee97-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="6ee97-104">Verwenden Sie zum vollständigen verwalten synchronisierter Benutzer und aller Attribute Ihre lokale Active Directory-Benutzer-und Gruppen Verwaltungskonsole (AdsiEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="6ee97-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="6ee97-105">Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in den folgenden allgemeinen Beispielen gezeigt:</span><span class="sxs-lookup"><span data-stu-id="6ee97-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
