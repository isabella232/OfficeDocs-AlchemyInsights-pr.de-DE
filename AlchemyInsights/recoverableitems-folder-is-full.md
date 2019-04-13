---
title: 1336 RecoverableItems-Ordner ist voll
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858995"
---
# <a name="the-recoverable-items-folder-is-full"></a>Der Ordner "Wiederherstellbare Elemente" ist voll

Bei Exchange Online-Postfächern in Office 365 beträgt der Standardspeichergrenzwert für den Ordner "Wiederherstellbare Elemente" 30 GB. Die Speichergrenzwerte für den Ordner "Wiederherstellbare Elemente" werden automatisch auf 100 GB erhöht, wenn das Postfach in der Warteschleife, in der eDiscovery-Speicherung oder einer Office 365-Aufbewahrungsrichtlinie zugewiesen ist.

Wenn der Ordner "Wiederherstellbare Elemente" den Speichergrenzwert erreicht, hat die Post Fach Funktionalität folgende Auswirkungen:

- Der Benutzer kann keine Elemente aus dem Postfach löschen.

- Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.

- Bei Postfächern, für die die Wiederherstellung einzelner Elemente aktiviert ist oder in der Warteschleife gespeichert ist, kann der Schutzprozess für die Kopie bei Schreibvorgang keine Versionen der Elemente verwalten, die vom Benutzer bearbeitet wurden.

- Bei Postfächern, für die die postfachüberwachungsprotokollierung aktiviert ist, können im Ordner "Wiederherstellbare Elemente" im Unterordner "Überwachungen" keine Einträge im postfachüberwachungsprotokoll gespeichert werden.

Bei Postfächern, die nicht in der Warteschleife sind `Search-Mailbox -SearchDumpsterOnly -DeleteContent` , können Administratoren den Befehl in Exchange Online PowerShell verwenden, um Elemente im Ordner "Wiederherstellbare Elemente" zu löschen. Weitere Informationen hierzu finden Sie in den folgenden Themen: 

- [Suchen nach und Löschen von Nachrichten](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Bei Postfächern, die in der Warteschleife sind, müssen Administratoren die Aufbewahrung entfernen, bevor Sie Elemente aus dem Ordner "Wiederherstellbare Elemente" löschen können. Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner "Wiederherstellbare Elemente" von Cloud-basierten Postfächern in der Warteschleife](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Um zu verhindern, dass der Ordner "Wiederherstellbare Elemente" vollständig wird, können Administratoren den Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" für Postfächer in der Warteschleife verlängern und eine Post Fach Aufbewahrungsrichtlinie einrichten, die Elemente aus dem Ordner "Wiederherstellbare Elemente" in das Archiv des Benutzers verschiebt. Post Fach. Weitere Informationen finden Sie unter [increase the recoverAble Items Quota for Mailboxes on Hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
