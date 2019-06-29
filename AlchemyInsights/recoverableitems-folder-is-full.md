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
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="34fd3-102">Der Ordner "refundable Items" ist voll</span><span class="sxs-lookup"><span data-stu-id="34fd3-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="34fd3-103">Für Exchange Online Postfächer in Office 365 beträgt der Standardspeichergrenzwert für den Ordner "refundable Items" 30 GB.</span><span class="sxs-lookup"><span data-stu-id="34fd3-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="34fd3-104">Der Speichergrenzwert für den Ordner "refundable Items" wird automatisch auf 100 GB erhöht, wenn das Postfach auf das Beweissicherungsverfahren, das eDiscovery-Archiv oder auf eine Office 365-Aufbewahrungsrichtlinie festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="34fd3-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="34fd3-105">Wenn der Ordner "refundable Items" den Speichergrenzwert erreicht, sind die Postfachfunktionen auf folgende Weise betroffen:</span><span class="sxs-lookup"><span data-stu-id="34fd3-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="34fd3-106">Der Benutzer kann keine Elemente aus dem Postfach löschen.</span><span class="sxs-lookup"><span data-stu-id="34fd3-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="34fd3-107">Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.</span><span class="sxs-lookup"><span data-stu-id="34fd3-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="34fd3-108">Bei Postfächern, für die die Wiederherstellung einzelner Elemente aktiviert ist oder in die Warteschleife gestellt wird, kann der Prozess zum Schutz durch Copy-on-Write-Seiten keine Versionen von Elementen verwalten, die vom Benutzer bearbeitet wurden.</span><span class="sxs-lookup"><span data-stu-id="34fd3-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="34fd3-109">Für Postfächer, für die die postfachüberwachungsprotokollierung aktiviert ist, können im Ordner "Wiederherstellbare Elemente" keine postfachüberwachungsprotokoll Einträge im Unterordner "Überwachungen" gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="34fd3-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="34fd3-110">Für Postfächer, die nicht in der Warteschleife sind, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` können Administratoren den Befehl in Exchange Online PowerShell verwenden, um Elemente im Ordner "Wiederherstellbare Elemente" zu löschen.</span><span class="sxs-lookup"><span data-stu-id="34fd3-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="34fd3-111">Weitere Informationen hierzu finden Sie in den folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="34fd3-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="34fd3-112">Suchen nach und Löschen von Nachrichten</span><span class="sxs-lookup"><span data-stu-id="34fd3-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="34fd3-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="34fd3-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="34fd3-114">Für Postfächer, die in der Warteschleife sind, müssen Administratoren den Haltebereich entfernen, bevor Sie Elemente aus dem Ordner "refundable Items" löschen können.</span><span class="sxs-lookup"><span data-stu-id="34fd3-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="34fd3-115">Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner "Wiederherstellbare Elemente" von cloudbasierten Postfächern in der Warteschleife](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="34fd3-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="34fd3-116">Um zu verhindern, dass der Ordner "Wiederherstellbare Elemente" vollständig wird, können Administratoren den Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" für Postfächer in der Warteschleife verbessern und eine Post Fach Aufbewahrungsrichtlinie einrichten, mit der Elemente aus dem Ordner "Wiederherstellbare Elemente" in das Archiv des Benutzers verschoben werden. Postfach.</span><span class="sxs-lookup"><span data-stu-id="34fd3-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="34fd3-117">Weitere Informationen finden Sie unter [Erweitern des Kontingents für die refundable Items für Postfächer, die aufbewahrt](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)werden</span><span class="sxs-lookup"><span data-stu-id="34fd3-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
