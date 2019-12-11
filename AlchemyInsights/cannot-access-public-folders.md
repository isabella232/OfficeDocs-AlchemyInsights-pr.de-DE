---
title: Zugriff auf Öffentliche Ordner nicht möglich
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959494"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="30872-102">Outlook kann keine Verbindung zu öffentlichen Ordnern herstellen</span><span class="sxs-lookup"><span data-stu-id="30872-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="30872-103">Wenn der Zugriff auf Öffentliche Ordner nicht für wenige Benutzer funktioniert, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="30872-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="30872-104">Stellen Sie eine Verbindung mit Exo PowerShell her, und konfigurieren Sie die DefaultPublicFolderMailbox für das Problem Benutzerkonto so, dass Sie mit einem Konto in einem funktionierenden Benutzerkonto übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="30872-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="30872-105">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="30872-105">Example:</span></span>

<span data-ttu-id="30872-106">Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="30872-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="30872-107">Festlegen-Postfach ProblemUser-DefaultPublicFolderMailbox \<-Wert aus dem vorherigen Befehls></span><span class="sxs-lookup"><span data-stu-id="30872-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="30872-108">Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="30872-108">Wait at least one hour for the change to take effect.</span></span>