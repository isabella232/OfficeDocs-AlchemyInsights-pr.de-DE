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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380504"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="98b61-102">Primäre e-Mail-Adresse kann nicht festgelegt oder Benutzerattribute geändert werden</span><span class="sxs-lookup"><span data-stu-id="98b61-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="98b61-103">Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer-oder Objektattribute nicht mithilfe des Admin Centers geändert werden.</span><span class="sxs-lookup"><span data-stu-id="98b61-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="98b61-104">Verwenden Sie zum vollständigen verwalten synchronisierter Benutzer und aller Attribute Ihre lokale Active Directory-Benutzer-und Gruppen Verwaltungskonsole (AdsiEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="98b61-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="98b61-105">Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in den folgenden allgemeinen Beispielen gezeigt:</span><span class="sxs-lookup"><span data-stu-id="98b61-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="98b61-106">Gruppe-MsolUser-userPrincipalName User@yourdomain.onmicrosoft.com-AlternateEmailAddresses User2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="98b61-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="98b61-107">Sets-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com"-DisplayName "Test User"-Nachname "User"-Titel "Manager"-Abteilung "HR"</span><span class="sxs-lookup"><span data-stu-id="98b61-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="98b61-108">Remove-MsolUser-userPrincipalName "User@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="98b61-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>