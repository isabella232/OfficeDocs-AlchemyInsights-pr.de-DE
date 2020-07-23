---
title: Problembehandlung bei der Kennwortsynchronisierung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387876"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="2c31f-102">Problembehandlung bei der Kennwortsynchronisierung</span><span class="sxs-lookup"><span data-stu-id="2c31f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="2c31f-103">Zur Behandlung von Problemen mit der Kennwortsynchronisierung beginnen Sie mit dieser Aad Connect-Problem Behandlungs Aufgabe, um zu ermitteln, warum Kennwörter nicht synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="2c31f-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="2c31f-104">Wechseln Sie zunächst zu [Manage Direct Sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="2c31f-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="2c31f-105">Öffnen Sie auf dem Azure AD Connect-Server eine neue Windows PowerShell-Sitzung, und wählen Sie die Option **als Administrator ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="2c31f-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="2c31f-106">Führen Sie "ExecutionPolicy RemoteSigned" oder "festgelegt-ExecutionPolicy Unrestricted" aus.</span><span class="sxs-lookup"><span data-stu-id="2c31f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="2c31f-107">Starten Sie den Azure AD Connect-Assistenten.</span><span class="sxs-lookup"><span data-stu-id="2c31f-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="2c31f-108">Wechseln Sie zur Seite Weitere Aufgaben > **Problembehandlung**  >  **als nächstes**.</span><span class="sxs-lookup"><span data-stu-id="2c31f-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="2c31f-109">Wählen Sie **Start** aus, um das PowerShell-Problem Behandlungs Menü zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="2c31f-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="2c31f-110">Wählen Sie **Problembehandlung bei der Kennwortsynchronisierung**aus.</span><span class="sxs-lookup"><span data-stu-id="2c31f-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="2c31f-111">Das Problem besteht in der Regel darin, dass ein Kennwort für ein bestimmtes Benutzerkonto nicht synchronisiert ist.</span><span class="sxs-lookup"><span data-stu-id="2c31f-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="2c31f-112">**Anmerkungen** Die Kennwortsynchronisierung schlägt fehl, wenn die letzte erfolgreiche Kennwortsynchronisierung vor einiger Zeit stattfand.</span><span class="sxs-lookup"><span data-stu-id="2c31f-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="2c31f-113">Weitere Hilfe zur Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennworthash Synchronisierung mit Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="2c31f-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>