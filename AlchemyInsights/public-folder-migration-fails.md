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
# <a name="public-folder-migration-fails-at-95"></a>Fehler bei der Migration öffentlicher Ordner bei 95 %

Möglicherweise haben Sie den Abschluss eines Migrationsbatch eingeleitet, und der Status des Migrationsbatches zeigt für lange Zeit den Status **Synchronisiert** an. Dieses Verhalten ist zu erwarten.

Es ist üblich, dass der Status eines Migrationsbatches einige Stunden lang auf **Synchronisiert** stehen bleibt, bevor er zu **Wird abgeschlossen** wechselt. Bei Migrationen mit einer großen Anzahl an Zielpostfächern ist es normal, dass der Status „synchronisiert“ länger als 24 Stunden zu sehen ist, solange keine der zugrunde liegenden Migrationsanforderungen öffentlicher Ordner fehlgeschlagen ist oder isoliert wurde. Bitte warten Sie 24-48 Stunden, bis im Migrationsbatch die Aufgaben abgeschlossen wurden.

Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:

1. Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.

2. Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.

3. Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.

4. Setzen Sie die Migration öffentlicher Ordner fort.
