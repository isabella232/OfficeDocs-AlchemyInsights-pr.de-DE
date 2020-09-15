---
title: Steuern des Zugriffs auf Öffentliche Ordner mit Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680485"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="dd40c-102">Steuern des Zugriffs auf Öffentliche Ordner mit Outlook</span><span class="sxs-lookup"><span data-stu-id="dd40c-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="dd40c-103">So steuern Sie, welche Benutzer über Outlook auf Öffentliche Ordner zugreifen können:</span><span class="sxs-lookup"><span data-stu-id="dd40c-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="dd40c-104">`Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` verwenden</span><span class="sxs-lookup"><span data-stu-id="dd40c-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="dd40c-105">$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook</span><span class="sxs-lookup"><span data-stu-id="dd40c-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="dd40c-106">$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook.</span><span class="sxs-lookup"><span data-stu-id="dd40c-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="dd40c-107">Dies ist der Standardwert.</span><span class="sxs-lookup"><span data-stu-id="dd40c-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="dd40c-108">Hinweis: Mit diesem Verfahren können nur Verbindungen mit dem Outlook-Desktop für Windows-Clients gesteuert werden.</span><span class="sxs-lookup"><span data-stu-id="dd40c-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="dd40c-109">Benutzer können weiterhin mit OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.</span><span class="sxs-lookup"><span data-stu-id="dd40c-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="dd40c-110">Weitere Informationen hierzu finden Sie unter [Kontrollierte Verbindungen zu Öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="dd40c-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
