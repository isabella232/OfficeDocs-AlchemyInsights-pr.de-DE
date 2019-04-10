---
title: Verschieben von e-Mail-Nachrichten in das Archivpostfach
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747202"
---
# <a name="move-email-to-the-archive-mailbox"></a>Verschieben von e-Mails in das Archivpostfach
 
1. Vergewissern Sie sich, dass ein **Archivpostfach** aktiviert wurde. Wenn nicht, führen Sie die Schritte in [diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) aus, um das Archivpostfach zu aktivieren.

2. Damit Nachrichten automatisch in das Archivpostfach archiviert werden, muss ein Aufbewahrungs mit der Aktion **in Archiv verschieben** so festgelegt werden, dass es **automatisch auf das gesamte Postfach (Standard) angewendet**wird. Führen Sie die folgenden Schritte aus, um das Tag: [Archive default-Tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)zu erstellen.
    
3. Als Nächstes fügen Sie das **Archiv** -Tag zu ihrer Aufbewahrungsrichtlinie hinzu. Wählen Sie im Exchange Admin Center **Aufbewahrungsrichtlinien** > Hinzufügen des **Tags Move to Archive** zur Richtlinie > **Speichern**. 
    
4. Weisen Sie jetzt die [Aufbewahrungsrichtlinie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) dem Postfach des jeweiligen Benutzers zu. Die gleiche Richtlinie wird sowohl auf das **primäre** als auch auf das **Archiv** Postfach angewendet. 
    
Möglicherweise müssen Sie erzwingen, dass der Assistent für verwaltete Ordner ausgeführt wird und die neuen Einstellungen auf das Postfach des Benutzers anwenden. Führen Sie den folgenden Befehl aus [, während Sie mit Exo PowerShell verbunden](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sind, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Weitere Informationen zum Einrichten einer Archivrichtlinie finden Sie unter [Einrichten einer Archiv-und Löschrichtlinie für Postfächer](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

