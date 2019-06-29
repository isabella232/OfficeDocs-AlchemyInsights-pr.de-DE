---
title: Aufbewahrungsrichtlinien im Exchange Admin Center funktionieren nicht
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369664"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Aufbewahrungsrichtlinien im Exchange Admin Center

 **Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien im Exchange Admin Center gelten nicht für Postfächer oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht. 
  
 **Ursachen:**
  
- Dies kann daran liegen, dass der **Assistent für verwaltete Ordner** das Postfach des Benutzers nicht verarbeitet hat. Der Assistent für verwaltete Ordner versucht, jedes Postfach in ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten. Wenn Sie ein Aufbewahrungs ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis die Unterstützung für verwaltete Ordner das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant ausführen, um den Assistenten für verwaltete Ordner zu starten, um einen bestimmten zu verarbeiten. Postfach. Das Ausführen dieses Cmdlets ist hilfreich zum Testen oder Problembehandlung einer Aufbewahrungsrichtlinie oder von Aufbewahrungstags Einstellungen. Weitere Informationen finden Sie unter [Ausführen des Assistenten für verwaltete Ordner](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dies kann auch auftreten, wenn **RetentionHold** für das Postfach **aktiviert** wurde. Wenn das Postfach auf einem RetentionHold gespeichert wurde, wird die Aufbewahrungsrichtlinie für das Postfach während dieser Zeit nicht verarbeitet. Weitere Informaton für die RetentionHold-Einstellung finden Sie unter: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lösung**
    
  - Überprüfen Sie den Status der RetentionHold-Einstellung für das jeweilige Postfach in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Führen Sie den folgenden Befehl aus, um RetentionHold für ein bestimmtes Postfach zu **Deaktivieren** :
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Führen Sie nun den Assistenten für verwaltete Ordner erneut aus:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, wird der Assistent für verwaltete Ordner das Postfach nicht automatisch verarbeiten.
  