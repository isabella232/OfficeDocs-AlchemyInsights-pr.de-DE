---
title: Für den Migrationsbatch für Öffentliche Ordner mit CompletedWithErrors Status
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043587"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="f2e13-102">Für den Migrationsbatch für Öffentliche Ordner mit CompletedWithErrors Status</span><span class="sxs-lookup"><span data-stu-id="f2e13-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="f2e13-103">Führen Sie die folgenden Schritte aus, um den Batch abzuschließen und die großen/schlechten Elemente zu überspringen:</span><span class="sxs-lookup"><span data-stu-id="f2e13-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="f2e13-104">Genehmigen der übersprungenen Elemente im Migrationsbatch:</span><span class="sxs-lookup"><span data-stu-id="f2e13-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="f2e13-105">Satz-MigrationBatch \<BatchName>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="f2e13-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="f2e13-106">Verwenden Sie den folgenden Befehl, um die übersprungenen Elemente für Migrationsanforderungen zu genehmigen, die "synchronisiert", aber nicht abgeschlossen sind:</span><span class="sxs-lookup"><span data-stu-id="f2e13-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="f2e13-107">$PF = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-Optionen Bericht einschließen; ForEach ($i in $PF) {if ($i. LargeItemsEncountered-gt 0-or $i. BadItemsEncountered-gt 0) {Sets-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="f2e13-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="f2e13-108">Der Migrationsbatch und die Anforderungen sollten in wenigen Minuten fortgesetzt und abgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="f2e13-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

