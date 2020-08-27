---
title: Fehler bei der Migration öffentlicher Ordner bei 95 %
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903564"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="27d79-102">Fehler bei der Migration öffentlicher Ordner bei 95 %</span><span class="sxs-lookup"><span data-stu-id="27d79-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="27d79-103">Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:</span><span class="sxs-lookup"><span data-stu-id="27d79-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="27d79-104">Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="27d79-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="27d79-105">Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.</span><span class="sxs-lookup"><span data-stu-id="27d79-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="27d79-106">Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.</span><span class="sxs-lookup"><span data-stu-id="27d79-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="27d79-107">Setzen Sie die Migration öffentlicher Ordner fort.</span><span class="sxs-lookup"><span data-stu-id="27d79-107">Resume public folder migration.</span></span>
