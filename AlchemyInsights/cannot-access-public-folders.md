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
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341402"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="b5fdf-102">Outlook kann keine Verbindung zu öffentlichen Ordnern herstellen</span><span class="sxs-lookup"><span data-stu-id="b5fdf-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="b5fdf-103">Wenn der Zugriff auf Öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="b5fdf-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="b5fdf-104">Stellen Sie eine Verbindung mit Exo PowerShell her, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das Problem Benutzerkonto so, dass er mit dem Parameter eines funktionierenden Benutzerkontos übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="b5fdf-105">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="b5fdf-105">Example:</span></span>

<span data-ttu-id="b5fdf-106">Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="b5fdf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="b5fdf-107">Festlegen-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="b5fdf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="b5fdf-108">Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="b5fdf-109">Wenn das Problem weiterhin besteht, führen Sie die folgenden [Schritte](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf Öffentliche Ordner mithilfe von Outlook zu beheben.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="b5fdf-110">**So steuern Sie, welche Benutzer mit Outlook auf Öffentliche Ordner zugreifen können**:</span><span class="sxs-lookup"><span data-stu-id="b5fdf-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="b5fdf-111">Verwenden Sie die $true oder $false von festlegen-CASMailbox <mailboxname> -PublicFolderClientAccess</span><span class="sxs-lookup"><span data-stu-id="b5fdf-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="b5fdf-112">$true: Benutzern den Zugriff auf Öffentliche Ordner in Outlook ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b5fdf-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="b5fdf-113">$false: verhindern des Benutzerzugriffs auf Öffentliche Ordner in Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="b5fdf-114">Dies ist der Standardwert.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="b5fdf-115">Gruppe-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="b5fdf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="b5fdf-116">**Hinweis:** Dieses Verfahren kann Verbindungen nur mit Outlook Desktop für Windows-Clients steuern.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="b5fdf-117">Ein Benutzer kann weiterhin mithilfe von OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.</span><span class="sxs-lookup"><span data-stu-id="b5fdf-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="b5fdf-118">Weitere Informationen finden Sie unter [Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="b5fdf-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>