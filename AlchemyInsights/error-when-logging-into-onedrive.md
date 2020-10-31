---
title: 0x8004de40-Fehler beim Starten von OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815992"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="a3b22-102">0x8004de40-Fehler beim Starten von OneDrive</span><span class="sxs-lookup"><span data-stu-id="a3b22-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="a3b22-103">Wenn beim Anmelden bei OneDrive ein Fehler **0x8004de40** angezeigt wird, starten Sie den Computer neu, während eine Verbindung mit ihrer Arbeits-oder Schul Domäne besteht.</span><span class="sxs-lookup"><span data-stu-id="a3b22-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="a3b22-104">Wenn Sie diesen Fehler nach dem Neustart erhalten, versuchen Sie Folgendes, während Sie mit ihrer geschäftlichen oder schulischen Domäne verbunden sind:</span><span class="sxs-lookup"><span data-stu-id="a3b22-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="a3b22-105">Klicken Sie auf Start, und geben Sie **cmd** oder **Eingabeaufforderung**  in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabe Aufforderungs-APP, und wählen Sie  **als Administrator ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="a3b22-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="a3b22-106">Wenn Sie zur Eingabe eines Administratorkennworts oder zur Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **zulassen** .</span><span class="sxs-lookup"><span data-stu-id="a3b22-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="a3b22-107">Geben Sie in das Eingabeaufforderungsfenster **dsregcmd/Leave**  ein, und warten Sie, bis der Befehl abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="a3b22-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="a3b22-108">Geben Sie dann **dsregcmd/Join** ein, und warten Sie, bis der Befehl abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="a3b22-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="a3b22-109">Starten Sie den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="a3b22-109">Reboot your computer.</span></span>
