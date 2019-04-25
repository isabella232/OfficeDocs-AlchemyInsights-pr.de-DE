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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389082"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="d34ad-102">Der Ordner "Wiederherstellbare Elemente" ist voll</span><span class="sxs-lookup"><span data-stu-id="d34ad-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="d34ad-103">Bei Exchange Online-Postfächern in Office 365 beträgt der Standardspeichergrenzwert für den Ordner "Wiederherstellbare Elemente" 30 GB.</span><span class="sxs-lookup"><span data-stu-id="d34ad-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="d34ad-104">Die Speichergrenzwerte für den Ordner "Wiederherstellbare Elemente" werden automatisch auf 100 GB erhöht, wenn das Postfach in der Warteschleife, in der eDiscovery-Speicherung oder einer Office 365-Aufbewahrungsrichtlinie zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="d34ad-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="d34ad-105">Wenn der Ordner "Wiederherstellbare Elemente" den Speichergrenzwert erreicht, hat die Post Fach Funktionalität folgende Auswirkungen:</span><span class="sxs-lookup"><span data-stu-id="d34ad-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="d34ad-106">Der Benutzer kann keine Elemente aus dem Postfach löschen.</span><span class="sxs-lookup"><span data-stu-id="d34ad-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="d34ad-107">Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.</span><span class="sxs-lookup"><span data-stu-id="d34ad-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="d34ad-108">Bei Postfächern, für die die Wiederherstellung einzelner Elemente aktiviert ist oder in der Warteschleife gespeichert ist, kann der Schutzprozess für die Kopie bei Schreibvorgang keine Versionen der Elemente verwalten, die vom Benutzer bearbeitet wurden.</span><span class="sxs-lookup"><span data-stu-id="d34ad-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="d34ad-109">Bei Postfächern, für die die postfachüberwachungsprotokollierung aktiviert ist, können im Ordner "Wiederherstellbare Elemente" im Unterordner "Überwachungen" keine Einträge im postfachüberwachungsprotokoll gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="d34ad-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="d34ad-110">Bei Postfächern, die nicht in der Warteschleife sind `Search-Mailbox -SearchDumpsterOnly -DeleteContent` , können Administratoren den Befehl in Exchange Online PowerShell verwenden, um Elemente im Ordner "Wiederherstellbare Elemente" zu löschen.</span><span class="sxs-lookup"><span data-stu-id="d34ad-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="d34ad-111">Weitere Informationen hierzu finden Sie in den folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="d34ad-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="d34ad-112">Suchen nach und Löschen von Nachrichten</span><span class="sxs-lookup"><span data-stu-id="d34ad-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="d34ad-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="d34ad-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="d34ad-114">Bei Postfächern, die in der Warteschleife sind, müssen Administratoren die Aufbewahrung entfernen, bevor Sie Elemente aus dem Ordner "Wiederherstellbare Elemente" löschen können.</span><span class="sxs-lookup"><span data-stu-id="d34ad-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="d34ad-115">Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner "Wiederherstellbare Elemente" von Cloud-basierten Postfächern in der Warteschleife](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="d34ad-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="d34ad-116">Um zu verhindern, dass der Ordner "Wiederherstellbare Elemente" vollständig wird, können Administratoren den Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" für Postfächer in der Warteschleife verlängern und eine Post Fach Aufbewahrungsrichtlinie einrichten, die Elemente aus dem Ordner "Wiederherstellbare Elemente" in das Archiv des Benutzers verschiebt. Post Fach.</span><span class="sxs-lookup"><span data-stu-id="d34ad-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="d34ad-117">Weitere Informationen finden Sie unter [increase the recoverAble Items Quota for Mailboxes on Hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="d34ad-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
