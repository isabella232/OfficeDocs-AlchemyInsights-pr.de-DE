---
title: Fehler bei der Migration öffentlicher Ordner bei 95 %
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662422"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="60ca2-102">Fehler bei der Migration öffentlicher Ordner bei 95 %</span><span class="sxs-lookup"><span data-stu-id="60ca2-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="60ca2-103">Möglicherweise haben Sie den Abschluss eines Migrationsbatch eingeleitet, und der Status des Migrationsbatches zeigt für lange Zeit den Status **Synchronisiert** an.</span><span class="sxs-lookup"><span data-stu-id="60ca2-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="60ca2-104">Dieses Verhalten ist zu erwarten.</span><span class="sxs-lookup"><span data-stu-id="60ca2-104">This is expected behavior.</span></span>

<span data-ttu-id="60ca2-105">Es ist üblich, dass der Status eines Migrationsbatches einige Stunden lang auf **Synchronisiert** stehen bleibt, bevor er zu **Wird abgeschlossen** wechselt.</span><span class="sxs-lookup"><span data-stu-id="60ca2-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="60ca2-106">Bei Migrationen mit einer großen Anzahl an Zielpostfächern ist es normal, dass der Status „synchronisiert“ länger als 24 Stunden zu sehen ist, solange keine der zugrunde liegenden Migrationsanforderungen öffentlicher Ordner fehlgeschlagen ist oder isoliert wurde.</span><span class="sxs-lookup"><span data-stu-id="60ca2-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="60ca2-107">Bitte warten Sie 24-48 Stunden, bis im Migrationsbatch die Aufgaben abgeschlossen wurden.</span><span class="sxs-lookup"><span data-stu-id="60ca2-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="60ca2-108">Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:</span><span class="sxs-lookup"><span data-stu-id="60ca2-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="60ca2-109">Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="60ca2-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="60ca2-110">Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.</span><span class="sxs-lookup"><span data-stu-id="60ca2-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="60ca2-111">Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.</span><span class="sxs-lookup"><span data-stu-id="60ca2-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="60ca2-112">Setzen Sie die Migration öffentlicher Ordner fort.</span><span class="sxs-lookup"><span data-stu-id="60ca2-112">Resume public folder migration.</span></span>
