---
title: Festlegen von ClientAccessServerEnabled auf True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736991"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="65e10-102">Festlegen von ClientAccessServerEnabled auf True</span><span class="sxs-lookup"><span data-stu-id="65e10-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="65e10-103">Wenn Sie keine verschlüsselte E-Mail-Nachricht öffnen und stattdessen eine **rpmsg-Anlage** sehen können, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="65e10-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="65e10-104">Stellen Sie eine Verbindung mit Exchange Online PowerShell her.</span><span class="sxs-lookup"><span data-stu-id="65e10-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="65e10-105">Um eine Verbindung mit Exchange Online PowerShell herzustellen, müssen Sie sich mit einem globalen Administrator- oder Exchange-Administratorkonto anmelden.</span><span class="sxs-lookup"><span data-stu-id="65e10-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="65e10-106">a.</span><span class="sxs-lookup"><span data-stu-id="65e10-106">a.</span></span> <span data-ttu-id="65e10-107">Öffnen Windows PowerShell, und führen Sie dann den folgenden Befehl aus: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="65e10-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="65e10-108">b.</span><span class="sxs-lookup"><span data-stu-id="65e10-108">b.</span></span> <span data-ttu-id="65e10-109">Geben Sie **im Windows PowerShell** Anmeldeinformationsanforderung Ihr Arbeits- oder Schulkonto und das Kennwort c ein.</span><span class="sxs-lookup"><span data-stu-id="65e10-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="65e10-110">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="65e10-110">Click **OK**.</span></span> 

2. <span data-ttu-id="65e10-111">Führen Sie den folgenden Befehl aus, um eine neue Sitzung zu erstellen:</span><span class="sxs-lookup"><span data-stu-id="65e10-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="65e10-112">a.</span><span class="sxs-lookup"><span data-stu-id="65e10-112">a.</span></span> <span data-ttu-id="65e10-113">Führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="65e10-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="65e10-114">Befehl `Get-IRMConfiguration` ausführen.</span><span class="sxs-lookup"><span data-stu-id="65e10-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="65e10-115">Überprüfen Sie die **Einstellung ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="65e10-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="65e10-116">a.</span><span class="sxs-lookup"><span data-stu-id="65e10-116">a.</span></span> <span data-ttu-id="65e10-117">Wenn **die Einstellung ClientAccessServerEnabled** auf **False festgelegt ist,** führen Sie das folgende Cmdlet aus: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="65e10-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="65e10-118">Schließen Sie Ihre powershell-Sitzung immer mit dem folgenden Befehl: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="65e10-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="65e10-119">Weitere Informationen finden Sie unter [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="65e10-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

