---
title: Ihr Archivpostfach ist fast voll
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950508"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="20516-102">Ihr Archivpostfach ist fast voll</span><span class="sxs-lookup"><span data-stu-id="20516-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="20516-103">Wenn der Benutzer die Warnung erhält; **Ihr Archivpostfach ist fast voll,** oder Sie müssen die Größe ihres Archivpostfachs erhöhen. Hier sind einige Tipps:</span><span class="sxs-lookup"><span data-stu-id="20516-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="20516-104">Wenn dem Benutzer ein Exchange Online Plan 1 zugewiesen ist, aktualisieren Sie auf **die Exchange Online Plan 2-Lizenz,** um die Größe von 50 GB auf 100 GB zu erhöhen.</span><span class="sxs-lookup"><span data-stu-id="20516-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="20516-105">Wenn dem Benutzer bereits einer der folgenden Optionen zugewiesen ist: **Exchange Online Plan 2** oder Exchange Online Plan 1 mit einem Exchange Online-Archivierung-Add-On, verwenden Sie die folgenden Schritte, um die Archivierung mit automatischer Erweiterung zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="20516-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="20516-106">[Stellen Sie eine Verbindung mit Exchange Online Powershell herstellen.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="20516-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="20516-107">Führen Sie das folgende Befehlslet für den Benutzer aus:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="20516-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="20516-108">Führen Sie das folgende Befehlslet aus, um zu bestätigen, dass es für den Benutzer aktiviert ist:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="20516-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="20516-109">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="20516-109">For more information see:</span></span>

- [<span data-ttu-id="20516-110"> Unbegrenzte Archivierung aktivieren – Administratorhilfe – Microsoft 365 Compliance | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="20516-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="20516-111">Exchange Online-Beschränkungen – Dienstbeschreibungen | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="20516-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="20516-112">Upgrade auf einen anderen Geschäftsplan | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="20516-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

