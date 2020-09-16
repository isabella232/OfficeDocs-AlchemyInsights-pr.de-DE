---
title: Kalenderberechtigungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748792"
---
# <a name="calendar-permissions"></a><span data-ttu-id="75f7d-102">Kalenderberechtigungen</span><span class="sxs-lookup"><span data-stu-id="75f7d-102">Calendar Permissions</span></span>

<span data-ttu-id="75f7d-103">Benutzer können Ihre eigenen Kalenderberechtigungen mit Outlook im Internet oder anderen Clients ändern, aber als Administrator müssen Sie möglicherweise auch untersuchen.</span><span class="sxs-lookup"><span data-stu-id="75f7d-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="75f7d-104">Mit dem Exchange PowerShell-Cmdlet wird Ihnen die Berechtigung für den Kalender eines Benutzers angezeigt:</span><span class="sxs-lookup"><span data-stu-id="75f7d-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="75f7d-105">Weitere Informationen finden Sie in den folgenden Themen:</span><span class="sxs-lookup"><span data-stu-id="75f7d-105">To see more information see the following:</span></span>

- [<span data-ttu-id="75f7d-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="75f7d-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="75f7d-107">Gruppe-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="75f7d-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="75f7d-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="75f7d-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="75f7d-109">Kalenderberechtigungen werden in der Freigabe von Kalendern verwendet, um weitere Informationen zur Freigabe eines Outlook-Kalenders zu erhalten, lesen Sie diese Artikel:</span><span class="sxs-lookup"><span data-stu-id="75f7d-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="75f7d-110">Freigeben eines Outlook-Kalenders für andere Personen</span><span class="sxs-lookup"><span data-stu-id="75f7d-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="75f7d-111">Freigeben Ihres Kalenders in Outlook im Internet für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="75f7d-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="75f7d-112">Zur Behandlung von Kalenderberechtigungen können Sie das [Unterstützungs-und Wiederherstellungs-Assistent](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) -Tool verwenden.</span><span class="sxs-lookup"><span data-stu-id="75f7d-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>