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
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt

Möglicherweise haben Sie den Abschluss des Migrationsbatch eingeleitet, und der Status des Migrationsbatch zeigt noch sehr lange "Synchronisiert" an. Dies ist ein erwartetes Verhalten.

Es ist üblich, dass der Migrationsbatchstatus einige Stunden lang auf Synchronisiert stehen bleibt, bevor er zu Wird abgeschlossen wechselt. Bei Migrationen mit einer großen Anzahl von Zielpostfächern ist es normal, dass der Status Synchronisiert länger als 24 Stunden zu sehen ist, sofern keine der zugrunde liegenden Migrationsanforderungen für öffentliche Ordner fehlgeschlagen ist oder isoliert wurde. Bitte warten Sie 24 - 48 Stunden, bis der Migrationsbatch die Aufgaben abgeschlossen hat.
