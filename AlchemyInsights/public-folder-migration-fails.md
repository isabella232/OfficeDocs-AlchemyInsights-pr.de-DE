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
ms.openlocfilehash: c1c4210baf93f0071a12f1902fb5f6fbf7bd0716
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341385"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="14c82-102">Fehler bei der Migration öffentlicher Ordner bei 95 %</span><span class="sxs-lookup"><span data-stu-id="14c82-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="14c82-103">Möglicherweise haben Sie den Abschluss eines Migrationsbatch eingeleitet, und der Status des Migrationsbatches zeigt für lange Zeit den Status **Synchronisiert** an.</span><span class="sxs-lookup"><span data-stu-id="14c82-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="14c82-104">Dieses Verhalten ist zu erwarten.</span><span class="sxs-lookup"><span data-stu-id="14c82-104">This is expected behavior.</span></span>

<span data-ttu-id="14c82-105">Es ist üblich, dass der Status eines Migrationsbatches einige Stunden lang auf **Synchronisiert** stehen bleibt, bevor er zu **Wird abgeschlossen** wechselt.</span><span class="sxs-lookup"><span data-stu-id="14c82-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="14c82-106">Bei Migrationen mit einer großen Anzahl an Zielpostfächern ist es normal, dass der Status „synchronisiert“ länger als 24 Stunden zu sehen ist, solange keine der zugrunde liegenden Migrationsanforderungen öffentlicher Ordner fehlgeschlagen ist oder isoliert wurde.</span><span class="sxs-lookup"><span data-stu-id="14c82-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="14c82-107">Bitte warten Sie 24-48 Stunden, bis im Migrationsbatch die Aufgaben abgeschlossen wurden.</span><span class="sxs-lookup"><span data-stu-id="14c82-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="14c82-108">Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:</span><span class="sxs-lookup"><span data-stu-id="14c82-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="14c82-109">Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="14c82-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="14c82-110">Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.</span><span class="sxs-lookup"><span data-stu-id="14c82-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="14c82-111">Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.</span><span class="sxs-lookup"><span data-stu-id="14c82-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="14c82-112">Setzen Sie die Migration öffentlicher Ordner fort.</span><span class="sxs-lookup"><span data-stu-id="14c82-112">Resume public folder migration.</span></span>
