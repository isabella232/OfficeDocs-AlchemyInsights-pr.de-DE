---
title: 1336 RecoverableItems Ordner ist voll.
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469980"
---
# <a name="the-recoverable-items-folder-is-full"></a>Ordner "wiederherstellbare Elemente" ist voll

Für Exchange Online-Postfächern in Office 365 ist der Standard-Speichergrenzwert für "wiederherstellbare Elemente" 30 GB. Der Speichergrenzwert für "wiederherstellbare Elemente" wird automatisch auf 100 GB erhöht, wenn das Postfach auf die Aufbewahrung für eventuelle Rechtsstreitigkeiten, eDiscovery-Archiv platziert wird oder eine Aufbewahrungsrichtlinie für Office 365 zugewiesen ist.
  
Wenn "wiederherstellbare Elemente" den Speichergrenzwert erreicht, wird die postfachfunktionalität auf folgende Weise beeinflusst:
  
- Der Benutzer kann nicht Elemente aus dem Postfach gelöscht werden.
    
- Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.
    
- Für Postfächer, die Wiederherstellung der einzelnen Elemente aktiviert oder in der Warteschleife platziert werden, kann nicht der Kopie bei Schreibvorgang Seite Protection Prozess Versionen von Elementen, die vom Benutzer bearbeitet verwalten.
    
- Postfächer, die Postfach-überwachungsprotokollierung aktiviert haben, können keine postfachüberwachungsprotokolleinträge im Überwachungen Unterordner im Ordner "wiederherstellbare Elemente" gespeichert werden.
    
Für Postfächer, die nicht in der Warteschleife sind, können Administratoren die `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Command in Exchange Online PowerShell, Elemente im Ordner "wiederherstellbare Elemente" zu löschen. Weitere Informationen finden Sie unter den folgenden Themen: 
  
- [Suchen nach und Löschen von Nachrichten](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Für Postfächer, die in der Warteschleife sind, müssen Administratoren sie gelöschte Elemente aus dem Ordner wiederherstellbare Elemente können die Sperre aufheben. Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner des cloudbasierten Postfächer auf halten wiederherstellbaren Elementen](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Zum Verhindern des Ordners wiederherstellbare Elemente voll können Administratoren erhöhen den Speichergrenzwert wiederherstellbaren Elementen für Postfächer auf Ordner halten, und richten Sie eine Postfachrichtlinie für die Aufbewahrung, die Elemente aus dem Ordner wiederherstellbare Elemente in das benutzerarchiv verschiebt Postfach. Finden Sie unter [Erhöhen der wiederherstellbare Elemente Kontingent für Postfächer auf halten](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

