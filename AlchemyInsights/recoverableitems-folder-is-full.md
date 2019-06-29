---
title: 1336 RecoverableItems-Ordner ist voll
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370386"
---
# <a name="the-recoverable-items-folder-is-full"></a>Der Ordner "refundable Items" ist voll

Für Exchange Online Postfächer in Office 365 beträgt der Standardspeichergrenzwert für den Ordner "refundable Items" 30 GB. Der Speichergrenzwert für den Ordner "refundable Items" wird automatisch auf 100 GB erhöht, wenn das Postfach auf das Beweissicherungsverfahren, das eDiscovery-Archiv oder auf eine Office 365-Aufbewahrungsrichtlinie festgelegt wird.

Wenn der Ordner "refundable Items" den Speichergrenzwert erreicht, sind die Postfachfunktionen auf folgende Weise betroffen:

- Der Benutzer kann keine Elemente aus dem Postfach löschen.

- Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.

- Bei Postfächern, für die die Wiederherstellung einzelner Elemente aktiviert ist oder in die Warteschleife gestellt wird, kann der Prozess zum Schutz durch Copy-on-Write-Seiten keine Versionen von Elementen verwalten, die vom Benutzer bearbeitet wurden.

- Für Postfächer, für die die postfachüberwachungsprotokollierung aktiviert ist, können im Ordner "Wiederherstellbare Elemente" keine postfachüberwachungsprotokoll Einträge im Unterordner "Überwachungen" gespeichert werden.

Für Postfächer, die nicht in der Warteschleife sind, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` können Administratoren den Befehl in Exchange Online PowerShell verwenden, um Elemente im Ordner "Wiederherstellbare Elemente" zu löschen. Weitere Informationen hierzu finden Sie in den folgenden Themen:

- [Suchen nach und Löschen von Nachrichten](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Für Postfächer, die in der Warteschleife sind, müssen Administratoren den Haltebereich entfernen, bevor Sie Elemente aus dem Ordner "refundable Items" löschen können. Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner "Wiederherstellbare Elemente" von cloudbasierten Postfächern in der Warteschleife](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Um zu verhindern, dass der Ordner "Wiederherstellbare Elemente" vollständig wird, können Administratoren den Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" für Postfächer in der Warteschleife verbessern und eine Post Fach Aufbewahrungsrichtlinie einrichten, mit der Elemente aus dem Ordner "Wiederherstellbare Elemente" in das Archiv des Benutzers verschoben werden. Postfach. Weitere Informationen finden Sie unter [Erweitern des Kontingents für die refundable Items für Postfächer, die aufbewahrt](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)werden
