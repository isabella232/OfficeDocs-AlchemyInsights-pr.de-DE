---
title: Behandlung von Problemen beim PST-Import
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991236"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="5be81-102">Behandlung von Problemen beim PST-Import</span><span class="sxs-lookup"><span data-stu-id="5be81-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="5be81-103">Wenn Sie innerhalb des Outlook-Clients importieren, lesen Sie [Beheben von Problemen beim Importieren einer PST-Datei in Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="5be81-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="5be81-104">Wenn Sie den Importdienst verwenden und er hängen bleibt, beachten Sie bitte, dass jede in den Azure-Speicherort hochgeladene PST-Datei nicht größer als 20 GB sein sollte.</span><span class="sxs-lookup"><span data-stu-id="5be81-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="5be81-105">PST-Dateien mit mehr als 20 GB können sich auf die Leistung des PST-Importprozesses auswirken.</span><span class="sxs-lookup"><span data-stu-id="5be81-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="5be81-106">Wenn Sie den Status eines bestimmten Importauftrags überprüfen möchten, können Sie [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) verwenden.</span><span class="sxs-lookup"><span data-stu-id="5be81-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="5be81-107">Ausführliche Informationen zum Importdienst finden Sie unter [Übersicht über das Importieren der PST-Dateien Ihrer Organisation](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="5be81-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
