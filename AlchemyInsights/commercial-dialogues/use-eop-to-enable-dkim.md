---
title: Verwenden von Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736912"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="efb94-102">Verwenden von Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne</span><span class="sxs-lookup"><span data-stu-id="efb94-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="efb94-103">Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, versuchen Sie es mit Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="efb94-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="efb94-104">Führen Sie die folgenden Schritte aus, um einen DKIM-DNS-Eintrag mit Exchange Online PowerShell zu erstellen:</span><span class="sxs-lookup"><span data-stu-id="efb94-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="efb94-105">Öffnen Windows PowerShell als Administrator, und führen Sie die folgenden Befehle in der beschriebenen Reihenfolge aus:</span><span class="sxs-lookup"><span data-stu-id="efb94-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="efb94-106">a.</span><span class="sxs-lookup"><span data-stu-id="efb94-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="efb94-107">b.</span><span class="sxs-lookup"><span data-stu-id="efb94-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="efb94-108">c.</span><span class="sxs-lookup"><span data-stu-id="efb94-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="efb94-109">Wenn Sie Probleme beim Herstellen einer Verbindung mit Exchange Online PowerShell haben, lesen Sie [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="efb94-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="efb94-110">Führen Sie nach der Verbindung mit Exchange Online PowerShell den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="efb94-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="efb94-111">Nachdem der obige Befehl erfolgreich ausgeführt wurde, führen Sie den folgenden Befehl aus, um die Exchange Online PowerShell-Sitzung zu beenden:</span><span class="sxs-lookup"><span data-stu-id="efb94-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



