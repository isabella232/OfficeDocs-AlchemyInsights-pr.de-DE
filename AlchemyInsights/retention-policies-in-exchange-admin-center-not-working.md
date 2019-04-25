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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="43dca-102">AufbewahrungsRichtlinien im Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="43dca-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="43dca-103">**Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien in der Exchange-Verwaltungskonsole gelten nicht für Postfächer, oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht.</span><span class="sxs-lookup"><span data-stu-id="43dca-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="43dca-104">**Ursachen:**</span><span class="sxs-lookup"><span data-stu-id="43dca-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="43dca-105">Möglicherweise hat der **Assistent für verwaltete Ordner** das Postfach des Benutzers nicht verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="43dca-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="43dca-106">Der Assistent für verwaltete Ordner versucht, jedes Postfach in ihrer cloudbasierten Organisation alle sieben Tage zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="43dca-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="43dca-107">Wenn Sie ein Aufbewahrungs ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis der Assistent für verwaltete Ordner das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant ausführen, um den Assistenten für verwaltete Ordner zu starten, um einen bestimmten Post Fach.</span><span class="sxs-lookup"><span data-stu-id="43dca-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="43dca-108">Die Verwendung dieses Cmdlets eignet sich zum Testen oder zur Problembehandlung einer Aufbewahrungsrichtlinie oder eines Aufbewahrungstags.</span><span class="sxs-lookup"><span data-stu-id="43dca-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="43dca-109">Weitere Informationen finden Sie unter [Ausführen des Assistenten für verwaltete Ordner](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="43dca-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="43dca-110">**Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:</span><span class="sxs-lookup"><span data-stu-id="43dca-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="43dca-111">Dies kann auch auftreten, wenn **RetentionHold** für das Postfach **aktiviert** wurde.</span><span class="sxs-lookup"><span data-stu-id="43dca-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="43dca-112">Wenn das Postfach auf einem RetentionHold wurde, wird die Aufbewahrungsrichtlinie für das Postfach zu diesem Zeitpunkt nicht verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="43dca-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="43dca-113">Weitere Informaton für die RetentionHold-Einstellung finden Sie unter: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="43dca-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="43dca-114">**Lösung**</span><span class="sxs-lookup"><span data-stu-id="43dca-114">**Solution:**</span></span>
    
  - <span data-ttu-id="43dca-115">Überprüfen Sie den Status der RetentionHold-Einstellung für das jeweilige Postfach in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="43dca-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="43dca-116">Führen Sie den folgenden Befehl aus, um RetentionHold für ein bestimmtes Postfach zu **Deaktivieren** :</span><span class="sxs-lookup"><span data-stu-id="43dca-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="43dca-117">Führen Sie nun den Assistenten für verwaltete Ordner erneut aus:</span><span class="sxs-lookup"><span data-stu-id="43dca-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="43dca-118">**Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, verarbeitet der Assistent für verwaltete Ordner das Postfach nicht automatisch.</span><span class="sxs-lookup"><span data-stu-id="43dca-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

