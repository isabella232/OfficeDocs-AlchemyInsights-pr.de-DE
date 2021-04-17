---
title: Kalenderberechtigungen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819907"
---
# <a name="calendar-permissions"></a><span data-ttu-id="edbd0-102">Kalenderberechtigungen</span><span class="sxs-lookup"><span data-stu-id="edbd0-102">Calendar Permissions</span></span>

<span data-ttu-id="edbd0-103">Benutzer können ihre eigenen Kalenderberechtigungen mit Outlook im Web oder anderen Clients ändern, aber als Administrator müssen Sie möglicherweise auch untersuchen.</span><span class="sxs-lookup"><span data-stu-id="edbd0-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="edbd0-104">Mit dem Exchange PowerShell-Cmdlet erhalten Sie die Berechtigung für den Kalender eines Benutzers:</span><span class="sxs-lookup"><span data-stu-id="edbd0-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="edbd0-105">Weitere Informationen finden Sie in den folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="edbd0-105">To see more information see the following:</span></span>

- [<span data-ttu-id="edbd0-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="edbd0-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="edbd0-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="edbd0-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="edbd0-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="edbd0-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="edbd0-109">Kalenderberechtigungen werden bei der Freigabe von Kalendern verwendet, um weitere Informationen zum Freigeben eines Outlook-Kalenders zu erhalten, finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="edbd0-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="edbd0-110">Freigeben eines Outlook-Kalenders für andere Personen</span><span class="sxs-lookup"><span data-stu-id="edbd0-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="edbd0-111">Freigeben Ihres Kalenders in Outlook im Web für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="edbd0-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="edbd0-112">Zur Problembehandlung von Kalenderberechtigungen können Sie das [Tool Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) verwenden.</span><span class="sxs-lookup"><span data-stu-id="edbd0-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>