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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Für den Migrationsbatch für Öffentliche Ordner mit CompletedWithErrors Status

Führen Sie die folgenden Schritte aus, um den Batch abzuschließen und die großen/schlechten Elemente zu überspringen: 
1. Genehmigen der übersprungenen Elemente im Migrationsbatch:

    Satz-MigrationBatch \<BatchName>-ApproveSkippedItems 
2. Verwenden Sie den folgenden Befehl, um die übersprungenen Elemente für Migrationsanforderungen zu genehmigen, die "synchronisiert", aber nicht abgeschlossen sind:

    $PF = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-Optionen Bericht einschließen; ForEach ($i in $PF) {if ($i. LargeItemsEncountered-gt 0-or $i. BadItemsEncountered-gt 0) {Sets-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}
3. Der Migrationsbatch und die Anforderungen sollten in wenigen Minuten fortgesetzt und abgeschlossen werden.

