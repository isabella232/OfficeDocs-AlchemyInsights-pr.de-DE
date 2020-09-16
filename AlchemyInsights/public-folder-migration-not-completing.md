---
title: Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt
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
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771487"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="cfbbf-102">Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt</span><span class="sxs-lookup"><span data-stu-id="cfbbf-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="cfbbf-103">Möglicherweise haben Sie den Abschluss des Migrationsbatch eingeleitet, und der Status des Migrationsbatch zeigt noch sehr lange "Synchronisiert" an.</span><span class="sxs-lookup"><span data-stu-id="cfbbf-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="cfbbf-104">Dies ist ein erwartetes Verhalten.</span><span class="sxs-lookup"><span data-stu-id="cfbbf-104">This is expected behavior.</span></span>

<span data-ttu-id="cfbbf-105">Es ist üblich, dass der Migrationsbatchstatus einige Stunden lang auf Synchronisiert stehen bleibt, bevor er zu Wird abgeschlossen wechselt.</span><span class="sxs-lookup"><span data-stu-id="cfbbf-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="cfbbf-106">Bei Migrationen mit einer großen Anzahl von Zielpostfächern ist es normal, dass der Status Synchronisiert länger als 24 Stunden zu sehen ist, sofern keine der zugrunde liegenden Migrationsanforderungen für öffentliche Ordner fehlgeschlagen ist oder isoliert wurde.</span><span class="sxs-lookup"><span data-stu-id="cfbbf-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="cfbbf-107">Bitte warten Sie 24 - 48 Stunden, bis der Migrationsbatch die Aufgaben abgeschlossen hat.</span><span class="sxs-lookup"><span data-stu-id="cfbbf-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
