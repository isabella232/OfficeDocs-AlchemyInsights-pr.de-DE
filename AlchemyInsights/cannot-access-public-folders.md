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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891748"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="e4d60-102">Outlook kann keine Verbindung zu öffentlichen Ordnern herstellen</span><span class="sxs-lookup"><span data-stu-id="e4d60-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="e4d60-103">Wenn der Zugriff auf Öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="e4d60-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="e4d60-104">Stellen Sie eine Verbindung mit Exo PowerShell her, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das Problem Benutzerkonto so, dass er mit dem Parameter eines funktionierenden Benutzerkontos übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="e4d60-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="e4d60-105">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="e4d60-105">Example:</span></span>

<span data-ttu-id="e4d60-106">Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="e4d60-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="e4d60-107">Festlegen-Postfach ProblemUser-DefaultPublicFolderMailbox \<-Wert aus dem vorherigen Befehls></span><span class="sxs-lookup"><span data-stu-id="e4d60-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="e4d60-108">Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="e4d60-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="e4d60-109">Wenn das Problem weiterhin besteht, führen Sie die folgenden [Schritte](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf Öffentliche Ordner mithilfe von Outlook zu beheben.</span><span class="sxs-lookup"><span data-stu-id="e4d60-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>