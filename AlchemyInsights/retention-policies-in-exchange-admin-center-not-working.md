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
ms.openlocfilehash: 6c69511f6bcdad5793cd2473a20a2d168d2ac260
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660706"
---
 <span data-ttu-id="8c4c3-102">**Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien in der Exchange-Verwaltungskonsole sind nicht auf Postfächer anwenden oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8c4c3-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="8c4c3-103">**Ursachen:**</span><span class="sxs-lookup"><span data-stu-id="8c4c3-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="8c4c3-p101">Dies kann sein, da die- **Assistenten für verwaltete Ordner** nicht das Postfach des Benutzers verarbeitet wurden. Assistenten für verwaltete Ordner versucht, alle Postfächer in Ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten. Wenn Sie ein aufbewahrungstag zu ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis die verwaltete Ordner unterstützen das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant, um den Assistenten für verwaltete Ordner zum Verarbeiten von einer bestimmtes starten ausführen Postfach. Dieses Cmdlet eignet sich zum Testen oder zur Problembehandlung einer Aufbewahrungsrichtlinie oder Einstellungen. Weitere Informationen finden Sie auf [Assistenten für verwaltete Ordner ausgeführt](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="8c4c3-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="8c4c3-109">**Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:</span><span class="sxs-lookup"><span data-stu-id="8c4c3-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="8c4c3-p102">Dies kann auch sein, wenn **RetentionHold** für das Postfach **aktiviert** wurde. Wenn das Postfach auf einem RetentionHold versetzt wurde, wird die Aufbewahrungsrichtlinie für das Postfach nicht während dieser Zeiten verarbeitet werden. Weitere Hinweise zu den RetentionHold Einstellung finden Sie unter: [Mailbox Aufbewahrungszeit](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="8c4c3-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="8c4c3-113">**Lösung:**</span><span class="sxs-lookup"><span data-stu-id="8c4c3-113">**Solution:**</span></span>
    
  - <span data-ttu-id="8c4c3-114">Überprüfen Sie den Status der Einstellung RetentionHold auf dem spezifischen Postfach in [EXO Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="8c4c3-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="8c4c3-115">Führen Sie den folgenden Befehl zum **Deaktivieren der** RetentionHold auf ein bestimmtes Postfach:</span><span class="sxs-lookup"><span data-stu-id="8c4c3-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="8c4c3-116">Nun, führen Sie den verwalteten Ordner Assistent erneut aus:</span><span class="sxs-lookup"><span data-stu-id="8c4c3-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="8c4c3-117">**Hinweis:** Wenn ein Postfach auf weniger als 10 MB festgelegt ist, wird die Assistenten für verwaltete Ordner nicht automatisch das Postfach verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="8c4c3-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

