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
# <a name="calendar-permissions"></a>Kalenderberechtigungen

Benutzer können ihre eigenen Kalenderberechtigungen mit Outlook im Web oder anderen Clients ändern, aber als Administrator müssen Sie möglicherweise auch untersuchen.  
Mit dem Exchange PowerShell-Cmdlet erhalten Sie die Berechtigung für den Kalender eines Benutzers:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Weitere Informationen finden Sie in den folgenden Themen:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenderberechtigungen werden bei der Freigabe von Kalendern verwendet, um weitere Informationen zum Freigeben eines Outlook-Kalenders zu erhalten, finden Sie in den folgenden Artikeln:

- [Freigeben eines Outlook-Kalenders für andere Personen](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Freigeben Ihres Kalenders in Outlook im Web für Unternehmen](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Zur Problembehandlung von Kalenderberechtigungen können Sie das [Tool Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) verwenden.