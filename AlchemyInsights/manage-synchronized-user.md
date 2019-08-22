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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541988"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="fb83a-102">Primäre e-Mail-Adresse kann nicht festgelegt oder Benutzerattribute geändert werden</span><span class="sxs-lookup"><span data-stu-id="fb83a-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="fb83a-103">Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer-oder Objektattribute nicht mithilfe des Microsoft 365 Admin Center geändert werden.</span><span class="sxs-lookup"><span data-stu-id="fb83a-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="fb83a-104">Verwenden Sie zum vollständigen verwalten synchronisierter Benutzer und aller Attribute Ihre lokale Active Directory-Benutzer-und Gruppen Verwaltungskonsole (AdsiEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="fb83a-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="fb83a-105">Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in den folgenden allgemeinen Beispielen gezeigt:</span><span class="sxs-lookup"><span data-stu-id="fb83a-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="fb83a-106">Gruppe-MsolUser-userPrincipalName User@yourdomain.onmicrosoft.com-AlternateEmailAddresses User2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fb83a-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="fb83a-107">Sets-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com"-DisplayName "Test User"-Nachname "User"-Titel "Manager"-Abteilung "HR"</span><span class="sxs-lookup"><span data-stu-id="fb83a-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="fb83a-108">Remove-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fb83a-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>