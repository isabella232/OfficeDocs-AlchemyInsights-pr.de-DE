---
title: E-Mail-Nachrichten in das Archivpostfach migrieren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762364"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-Mail-Nachricht in das Archivpostfach migrieren
 
1. Stellen Sie sicher, dass ein **Archivpostfach** aktiviert wurde. Wenn dies nicht der Fall ist, verwenden Sie die Schritte in [diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , um das Archivpostfach zu aktivieren.

2. Um Nachrichten automatisch in das Archivpostfach zu archivieren, muss ein Aufbewahrungs mit der Aktion **in Archiv** verlegen auf **automatisch auf gesamtes Postfach (Standard) angewendet**werden. Verwenden Sie die Schritte hier, um das Tag: [Archive default-Tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)zu erstellen.
    
3. Fügen Sie als nächstes das **Archiv** -Tag zu ihrer Aufbewahrungsrichtlinie hinzu. Wählen Sie in der Exchange-Verwaltungskonsole die Option **Aufbewahrungsrichtlinien** #a0 fügen Sie der Richtlinie #a1 **Speichern**das **Element zum Archivieren** hinzu. 
    
4. [Weisen Sie die Aufbewahrungsrichtlinie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nun dem Postfach des jeweiligen Benutzers zu. Dieselbe Richtlinie wird sowohl auf das **primäre** als auch auf das **Archiv** Postfach angewendet. 
    
Es kann erforderlich sein, die Ausführung des Assistenten für verwaltete Ordner (MFA) zu erzwingen und die neuen Einstellungen auf das Postfach des Benutzers anzuwenden. Führen Sie den folgenden Befehl aus, während eine [Verbindung mit Exo PowerShell hergestellt](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) wurde, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Weitere Informationen zum Einrichten einer Archivrichtlinie finden Sie unter [Einrichten einer Archiv-und Löschrichtlinie für Postfächer](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

