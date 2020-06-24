---
title: Kalenderberechtigungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854009"
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