---
title: Die Standardauthentifizierung für Exchange PowerShell wird eingestellt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205194"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="87e51-102">Die Standardauthentifizierung für Exchange PowerShell wird eingestellt</span><span class="sxs-lookup"><span data-stu-id="87e51-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="87e51-103">Die neuesten Informationen darüber, wie eine Verbindung zu Exchange Online PowerShell ohne Verwendung der Standardauthentifizierung hergestellt werden kann, [finden Sie hier](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="87e51-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="87e51-104">Im PowerShell V2-Modul wird keine Standardauthentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="87e51-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="87e51-105">Beachten Sie, dass auf dem Clientcomputer weiterhin die Standardauthentifizierung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="87e51-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="87e51-106">Das neue PowerShell V2-Modul verwendet moderne Authentifizierung, um eine Verbindung zum Aktivieren aller REST-basierten V2-Cmdlets herzustellen.</span><span class="sxs-lookup"><span data-stu-id="87e51-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="87e51-107">Zusätzlich zu den V2-Cmdlets ermöglicht es Ihnen auch den Zugriff auf ältere Remote-PowerShell-Cmdlets (RPS), für die eine PowerShell-Remotesitzung eingerichtet werden muss.</span><span class="sxs-lookup"><span data-stu-id="87e51-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="87e51-108">Zum Einrichten einer RPS-Sitzung auf einem Windows-Computer muss WinRM BasicAuth auf dem Clientcomputer aktiviert werden, auch wenn das Modul einen modernen Authentifizierungsmechanismus für den Dienst verwendet.</span><span class="sxs-lookup"><span data-stu-id="87e51-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="87e51-109">Die WinRM-Standardauthentifizierungspipeline wird für den Transport moderner Authentifizierungstoken verwendet.</span><span class="sxs-lookup"><span data-stu-id="87e51-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="87e51-110">Wenn die WinRM-Standardauthentifizierung auf dem Clientcomputer deaktiviert ist, funktionieren die neuen V2-Cmdlets weiterhin (aber die alten RPS-Cmdlets nicht).</span><span class="sxs-lookup"><span data-stu-id="87e51-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
