---
title: Aufbewahrungsrichtlinien in Exchange-Verwaltungskonsole nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470283"
---
 **Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien in der Exchange-Verwaltungskonsole sind nicht auf Postfächer anwenden oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht. 
  
 **Ursachen:**
  
- Dies kann sein, da die- **Assistenten für verwaltete Ordner** nicht das Postfach des Benutzers verarbeitet wurden. Assistenten für verwaltete Ordner versucht, alle Postfächer in Ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten. Wenn Sie ein aufbewahrungstag zu ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis die verwaltete Ordner unterstützen das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant, um den Assistenten für verwaltete Ordner zum Verarbeiten von einer bestimmtes starten ausführen Postfach. Dieses Cmdlet eignet sich zum Testen oder zur Problembehandlung einer Aufbewahrungsrichtlinie oder Einstellungen. Weitere Informationen finden Sie auf [Assistenten für verwaltete Ordner ausgeführt](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dies kann auch sein, wenn **RetentionHold** für das Postfach **aktiviert** wurde. Wenn das Postfach auf einem RetentionHold versetzt wurde, wird die Aufbewahrungsrichtlinie für das Postfach nicht während dieser Zeiten verarbeitet werden. Weitere Hinweise zu den RetentionHold Einstellung finden Sie unter: [Mailbox Aufbewahrungszeit](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lösung**
    
  - Überprüfen Sie den Status der Einstellung RetentionHold auf dem spezifischen Postfach in [EXO Powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Führen Sie den folgenden Befehl zum **Deaktivieren der** RetentionHold auf ein bestimmtes Postfach: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nun, führen Sie den verwalteten Ordner Assistent erneut aus:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Hinweis:** Wenn ein Postfach auf weniger als 10 MB festgelegt ist, wird die Assistenten für verwaltete Ordner nicht automatisch das Postfach verarbeitet. 
  

