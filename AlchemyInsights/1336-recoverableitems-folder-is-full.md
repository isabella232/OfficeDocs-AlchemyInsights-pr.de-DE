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
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="5416c-102">Ordner "wiederherstellbare Elemente" ist voll</span><span class="sxs-lookup"><span data-stu-id="5416c-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="5416c-p101">Für Exchange Online-Postfächern in Office 365 ist der Standard-Speichergrenzwert für "wiederherstellbare Elemente" 30 GB. Der Speichergrenzwert für "wiederherstellbare Elemente" wird automatisch auf 100 GB erhöht, wenn das Postfach auf die Aufbewahrung für eventuelle Rechtsstreitigkeiten, eDiscovery-Archiv platziert wird oder eine Aufbewahrungsrichtlinie für Office 365 zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="5416c-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="5416c-105">Wenn "wiederherstellbare Elemente" den Speichergrenzwert erreicht, wird die postfachfunktionalität auf folgende Weise beeinflusst:</span><span class="sxs-lookup"><span data-stu-id="5416c-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="5416c-106">Der Benutzer kann nicht Elemente aus dem Postfach gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="5416c-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="5416c-107">Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.</span><span class="sxs-lookup"><span data-stu-id="5416c-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="5416c-108">Für Postfächer, die Wiederherstellung der einzelnen Elemente aktiviert oder in der Warteschleife platziert werden, kann nicht der Kopie bei Schreibvorgang Seite Protection Prozess Versionen von Elementen, die vom Benutzer bearbeitet verwalten.</span><span class="sxs-lookup"><span data-stu-id="5416c-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="5416c-109">Postfächer, die Postfach-überwachungsprotokollierung aktiviert haben, können keine postfachüberwachungsprotokolleinträge im Überwachungen Unterordner im Ordner "wiederherstellbare Elemente" gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="5416c-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="5416c-p102">Für Postfächer, die nicht in der Warteschleife sind, können Administratoren die `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Command in Exchange Online PowerShell, Elemente im Ordner "wiederherstellbare Elemente" zu löschen. Weitere Informationen finden Sie unter den folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="5416c-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="5416c-112">Suchen nach und Löschen von Nachrichten</span><span class="sxs-lookup"><span data-stu-id="5416c-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="5416c-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="5416c-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="5416c-p103">Für Postfächer, die in der Warteschleife sind, müssen Administratoren sie gelöschte Elemente aus dem Ordner wiederherstellbare Elemente können die Sperre aufheben. Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner des cloudbasierten Postfächer auf halten wiederherstellbaren Elementen](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="5416c-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="5416c-p104">Zum Verhindern des Ordners wiederherstellbare Elemente voll können Administratoren erhöhen den Speichergrenzwert wiederherstellbaren Elementen für Postfächer auf Ordner halten, und richten Sie eine Postfachrichtlinie für die Aufbewahrung, die Elemente aus dem Ordner wiederherstellbare Elemente in das benutzerarchiv verschiebt Postfach. Finden Sie unter [Erhöhen der wiederherstellbare Elemente Kontingent für Postfächer auf halten](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="5416c-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

