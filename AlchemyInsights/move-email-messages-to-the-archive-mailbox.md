---
title: Verschieben von e-Mail-Nachrichten in das Archivpostfach
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290170"
---
Probleme bei der Archivierung von Elementen in das Archivpostfach. Stellen Sie sicher, dass Sie die folgenden Schritte ausgeführt haben:
  
1. Vergewissern Sie sich, dass ein **archivieren Postfach** aktiviert wurde. Wenn dies nicht der Fall ist, verwenden Sie in [diesem Artikel](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) die Schritte aus, um das Archivpostfach aktivieren. 
    
2. Wählen Sie in der Exchange-Verwaltungskonsole **Retention Tags** unter **Verwaltung der Richtlinientreue**, erstellen Sie ein **aufbewahrungstag** mit der Aktion **in Archiv verschieben** , enthält das gewünschte **Aufbewahrungszeitraum**.
    
3. Klicken Sie in der Exchange-Verwaltungskonsole wählen Sie **Aufbewahrungsrichtlinien**, erstellen Sie eine **Aufbewahrungsrichtlinie** , und fügen Sie Ihrer aufbewahrungstag **in Archiv verschieben** dieser Richtlinie. 
    
4. Sie [weisen die Aufbewahrungsrichtlinie](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Postfach für den betreffenden Benutzer. Die gleiche Richtlinie wird auf **primäre** und **das Archivpostfach** angewendet werden. 
    
Das Postfach des Benutzers sollte jetzt eine Archivrichtlinie Elemente in das Archivpostfach verschieben. Möglicherweise erforderlich sind, um zu erzwingen, dass die verwaltete Ordner-Assistent (mehrstufiger Authentifizierung das) ausführen und die neuen Einstellungen auf das Postfach des Benutzers angewendet werden. Führen Sie den folgenden Befehl während [EXO PowerShell verbunden](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Möchten Sie weitere Informationen zum Einrichten einer Richtlinie für den archivieren, finden Sie unter [Set up ein Archiv und Löschung Richtlinie für Postfächer](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

