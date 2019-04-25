---
title: AufbewahrungsRichtlinien in Exchange Admin Center funktionieren nicht
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371297"
---
# <a name="retention-policies-in-exchange-admin-center"></a>AufbewahrungsRichtlinien im Exchange Admin Center

 **Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien in der Exchange-Verwaltungskonsole gelten nicht für Postfächer, oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht. 
  
 **Ursachen:**
  
- Möglicherweise hat der **Assistent für verwaltete Ordner** das Postfach des Benutzers nicht verarbeitet. Der Assistent für verwaltete Ordner versucht, jedes Postfach in ihrer cloudbasierten Organisation alle sieben Tage zu verarbeiten. Wenn Sie ein Aufbewahrungs ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis der Assistent für verwaltete Ordner das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant ausführen, um den Assistenten für verwaltete Ordner zu starten, um einen bestimmten Post Fach. Die Verwendung dieses Cmdlets eignet sich zum Testen oder zur Problembehandlung einer Aufbewahrungsrichtlinie oder eines Aufbewahrungstags. Weitere Informationen finden Sie unter [Ausführen des Assistenten für verwaltete Ordner](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dies kann auch auftreten, wenn **RetentionHold** für das Postfach **aktiviert** wurde. Wenn das Postfach auf einem RetentionHold wurde, wird die Aufbewahrungsrichtlinie für das Postfach zu diesem Zeitpunkt nicht verarbeitet. Weitere Informaton für die RetentionHold-Einstellung finden Sie unter: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
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

 **Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, verarbeitet der Assistent für verwaltete Ordner das Postfach nicht automatisch. 
  

