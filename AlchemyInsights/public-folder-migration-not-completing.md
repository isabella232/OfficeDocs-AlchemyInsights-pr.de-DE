---
title: Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt
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
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406570"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="c0fa7-102">Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt</span><span class="sxs-lookup"><span data-stu-id="c0fa7-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="c0fa7-103">Möglicherweise haben Sie den Abschluss des Migrationsbatch eingeleitet, und der Status des Migrationsbatch zeigt noch sehr lange "Synchronisiert" an.</span><span class="sxs-lookup"><span data-stu-id="c0fa7-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="c0fa7-104">Dies ist ein erwartetes Verhalten.</span><span class="sxs-lookup"><span data-stu-id="c0fa7-104">This is expected behavior.</span></span>

<span data-ttu-id="c0fa7-105">Es ist üblich, dass der Migrationsbatchstatus einige Stunden lang auf Synchronisiert stehen bleibt, bevor er zu Wird abgeschlossen wechselt.</span><span class="sxs-lookup"><span data-stu-id="c0fa7-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="c0fa7-106">Bei Migrationen mit einer großen Anzahl von Zielpostfächern ist es normal, dass der Status Synchronisiert länger als 24 Stunden zu sehen ist, sofern keine der zugrunde liegenden Migrationsanforderungen für öffentliche Ordner fehlgeschlagen ist oder isoliert wurde.</span><span class="sxs-lookup"><span data-stu-id="c0fa7-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="c0fa7-107">Bitte warten Sie 24 - 48 Stunden, bis der Migrationsbatch die Aufgaben abgeschlossen hat.</span><span class="sxs-lookup"><span data-stu-id="c0fa7-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
