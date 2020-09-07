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
# <a name="public-folder-migration-fails-at-95"></a>Fehler bei der Migration öffentlicher Ordner bei 95 %

Möglicherweise haben Sie den Abschluss eines Migrationsbatch eingeleitet, und der Status des Migrationsbatches zeigt für lange Zeit den Status **Synchronisiert** an. Dieses Verhalten ist zu erwarten.

Es ist üblich, dass der Status eines Migrationsbatches einige Stunden lang auf **Synchronisiert** stehen bleibt, bevor er zu **Wird abgeschlossen** wechselt. Bei Migrationen mit einer großen Anzahl an Zielpostfächern ist es normal, dass der Status „synchronisiert“ länger als 24 Stunden zu sehen ist, solange keine der zugrunde liegenden Migrationsanforderungen öffentlicher Ordner fehlgeschlagen ist oder isoliert wurde. Bitte warten Sie 24-48 Stunden, bis im Migrationsbatch die Aufgaben abgeschlossen wurden.

Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:

1. Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.

2. Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.

3. Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.

4. Setzen Sie die Migration öffentlicher Ordner fort.
