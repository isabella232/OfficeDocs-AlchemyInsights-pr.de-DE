---
title: Proxyadressenfehler beim Erstellen eines freigegebenen Postfachs
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568289"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="10efc-102">Proxyadressenfehler beim Erstellen eines Postfachs oder eines anderen E-Mail-aktivierten Objekts</span><span class="sxs-lookup"><span data-stu-id="10efc-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="10efc-103">Wenn Sie versucht haben, ein E-Mail-aktiviertes Objekt (Postfach, freigegebenes Postfach usw.) zu erstellen und den Fehler "Die Proxyadresse "SMTP:alias@domain.com" wird bereits verwendet..." erhalten, wird die E-Mail-Adresse, die Sie ausgewählt haben, bereits von einem anderen E-Mail-aktivierten Objekt in Ihrer Organisation übernommen.</span><span class="sxs-lookup"><span data-stu-id="10efc-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="10efc-104">Sie müssen den Benutzer, die Gruppe, das freigegebene Postfach oder den öffentlichen Ordner mit dieser E-Mail-Adresse suchen und löschen oder seine E-Mail-Adresse ändern.</span><span class="sxs-lookup"><span data-stu-id="10efc-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="10efc-105">Anschließend können Sie ein neues E-Mail-aktiviertes Objekt mit der freigegebenen E-Mail-Adresse erstellen.</span><span class="sxs-lookup"><span data-stu-id="10efc-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="10efc-106">Verwenden Sie die Suche auf der Startseite, um sie zu finden.</span><span class="sxs-lookup"><span data-stu-id="10efc-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="10efc-107">Sie können auch den folgenden Exchange Online PowerShell-Befehl verwenden, um danach zu suchen:</span><span class="sxs-lookup"><span data-stu-id="10efc-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="10efc-108">Wenn Sie die vorhandene E-Mail-Adresse nicht löschen möchten, wählen Sie eine neue E-Mail-Adresse für das neue Objekt aus, das Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="10efc-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  