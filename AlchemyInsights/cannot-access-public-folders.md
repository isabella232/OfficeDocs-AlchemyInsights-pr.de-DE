---
title: Zugriff auf öffentliche Ordner nicht möglich
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819511"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="41faf-102">Outlook kann keine Verbindung mit öffentlichen Ordnern herstellen</span><span class="sxs-lookup"><span data-stu-id="41faf-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="41faf-103">Wenn der Zugriff auf öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="41faf-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="41faf-104">Stellen Sie eine Verbindung mit EXO PowerShell ein, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das Problembenutzerkonto so, dass er mit dem Parameter für ein funktionierendes Benutzerkonto übereinstimmen kann.</span><span class="sxs-lookup"><span data-stu-id="41faf-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="41faf-105">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="41faf-105">Example:</span></span>

<span data-ttu-id="41faf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="41faf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="41faf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="41faf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="41faf-108">Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="41faf-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="41faf-109">Wenn das Problem weiterhin bestehen bleibt, führen Sie dieses Verfahren aus, [um](https://aka.ms/pfcte) Probleme mit dem Zugriff auf öffentliche Ordner mithilfe von Outlook zu beheben.</span><span class="sxs-lookup"><span data-stu-id="41faf-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="41faf-110">**So steuern Sie, welche Benutzer über Outlook auf öffentliche Ordner zugreifen können:**</span><span class="sxs-lookup"><span data-stu-id="41faf-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="41faf-111">Verwenden Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true oder $false</span><span class="sxs-lookup"><span data-stu-id="41faf-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="41faf-112">$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook</span><span class="sxs-lookup"><span data-stu-id="41faf-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="41faf-113">$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook.</span><span class="sxs-lookup"><span data-stu-id="41faf-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="41faf-114">Dies ist der Standardwert.</span><span class="sxs-lookup"><span data-stu-id="41faf-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="41faf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="41faf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="41faf-116">**Hinweis** Dieses Verfahren kann nur Verbindungen mit Outlook Desktop für Windows-Clients steuern.</span><span class="sxs-lookup"><span data-stu-id="41faf-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="41faf-117">Ein Benutzer kann weiterhin über OWA oder Outlook für Mac auf öffentliche Ordner zugreifen.</span><span class="sxs-lookup"><span data-stu-id="41faf-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="41faf-118">Weitere Informationen finden Sie unter [Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="41faf-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>