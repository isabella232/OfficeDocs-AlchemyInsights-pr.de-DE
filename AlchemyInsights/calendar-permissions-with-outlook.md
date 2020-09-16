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
# <a name="calendar-permissions"></a>Kalenderberechtigungen

Benutzer können Ihre eigenen Kalenderberechtigungen mit Outlook im Internet oder anderen Clients ändern, aber als Administrator müssen Sie möglicherweise auch untersuchen.  
Mit dem Exchange PowerShell-Cmdlet wird Ihnen die Berechtigung für den Kalender eines Benutzers angezeigt:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Weitere Informationen finden Sie in den folgenden Themen:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Gruppe-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenderberechtigungen werden in der Freigabe von Kalendern verwendet, um weitere Informationen zur Freigabe eines Outlook-Kalenders zu erhalten, lesen Sie diese Artikel:

- [Freigeben eines Outlook-Kalenders für andere Personen](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Freigeben Ihres Kalenders in Outlook im Internet für Unternehmen](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Zur Behandlung von Kalenderberechtigungen können Sie das [Unterstützungs-und Wiederherstellungs-Assistent](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) -Tool verwenden.