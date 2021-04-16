---
title: Für Migrationsbatch für öffentliche Ordner mit Dem Status CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812463"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="b02b9-102">Für Migrationsbatch für öffentliche Ordner mit Dem Status CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="b02b9-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="b02b9-103">Führen Sie die folgenden Schritte aus, um den Batch zu vervollständigen, und überspringen Sie die großen/ungültigen Elemente:</span><span class="sxs-lookup"><span data-stu-id="b02b9-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="b02b9-104">Genehmigen der übersprungenen Elemente im Migrationsbatch:</span><span class="sxs-lookup"><span data-stu-id="b02b9-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="b02b9-105">Verwenden Sie den folgenden Befehl, um die übersprungenen Elemente für Migrationsanforderungen zu genehmigen, die zwar synchronisiert, aber nicht abgeschlossen sind:</span><span class="sxs-lookup"><span data-stu-id="b02b9-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="b02b9-106">Der Migrationsbatch und die Anforderungen sollten in wenigen Minuten fortgesetzt und abgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="b02b9-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

