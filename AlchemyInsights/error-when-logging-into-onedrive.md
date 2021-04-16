---
title: 0x8004de40 fehler beim Starten von OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813651"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b643c-102">0x8004de40 fehler beim Starten von OneDrive</span><span class="sxs-lookup"><span data-stu-id="b643c-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b643c-103">Wenn bei der Anmeldung bei OneDrive **0x8004de40** Fehler angezeigt wird, starten Sie den Computer neu, während sie mit Ihrer Arbeits- oder Schuldomäne verbunden sind.</span><span class="sxs-lookup"><span data-stu-id="b643c-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b643c-104">Wenn Sie diesen Fehler nach dem Neustart erhalten, versuchen Sie dies, während Sie mit Ihrer Arbeits- oder Schuldomäne verbunden sind:</span><span class="sxs-lookup"><span data-stu-id="b643c-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b643c-105">Klicken Sie auf Start, und geben Sie **cmd** **oder** Eingabeaufforderung in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabeaufforderungs-App, und wählen Sie Als Administrator **ausführen aus.**</span><span class="sxs-lookup"><span data-stu-id="b643c-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="b643c-106">Wenn Sie zur Eingabe eines Administratorkennworts oder einer Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **Zulassen**.</span><span class="sxs-lookup"><span data-stu-id="b643c-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="b643c-107">Geben Sie im Eingabeaufforderungsfenster **dsregcmd /leave ein,**  und warten Sie, bis der Befehl abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="b643c-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b643c-108">Geben Sie dann **dsregcmd /join ein,** und warten Sie, bis der Befehl abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="b643c-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b643c-109">Starten Sie Ihren Computer neu.</span><span class="sxs-lookup"><span data-stu-id="b643c-109">Reboot your computer.</span></span>
