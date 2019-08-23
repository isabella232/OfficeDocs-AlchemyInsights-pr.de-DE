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
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551342"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="03211-102">Aufbewahrungsrichtlinien im Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="03211-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="03211-103">**Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien im Exchange Admin Center gelten nicht für Postfächer oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht.</span><span class="sxs-lookup"><span data-stu-id="03211-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="03211-104">**Ursachen:**</span><span class="sxs-lookup"><span data-stu-id="03211-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="03211-105">Dies kann daran liegen, dass der **Assistent für verwaltete Ordner** das Postfach des Benutzers nicht verarbeitet hat.</span><span class="sxs-lookup"><span data-stu-id="03211-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="03211-106">Der Assistent für verwaltete Ordner versucht, jedes Postfach in ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="03211-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="03211-107">Wenn Sie ein Aufbewahrungs ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis die Unterstützung für verwaltete Ordner das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant ausführen, um den Assistenten für verwaltete Ordner zu starten, um einen bestimmten zu verarbeiten. Postfach.</span><span class="sxs-lookup"><span data-stu-id="03211-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="03211-108">Das Ausführen dieses Cmdlets ist hilfreich zum Testen oder Problembehandlung einer Aufbewahrungsrichtlinie oder von Aufbewahrungstags Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="03211-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="03211-109">Weitere Informationen finden Sie unter [Ausführen des Assistenten für verwaltete Ordner](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="03211-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="03211-110">**Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:</span><span class="sxs-lookup"><span data-stu-id="03211-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="03211-111">Dies kann auch auftreten, wenn **RetentionHold** für das Postfach **aktiviert** wurde.</span><span class="sxs-lookup"><span data-stu-id="03211-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="03211-112">Wenn das Postfach auf einem RetentionHold gespeichert wurde, wird die Aufbewahrungsrichtlinie für das Postfach während dieser Zeit nicht verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="03211-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="03211-113">Weitere Informaton für die RetentionHold-Einstellung finden Sie unter: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="03211-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="03211-114">**Lösung**</span><span class="sxs-lookup"><span data-stu-id="03211-114">**Solution:**</span></span>
    
  - <span data-ttu-id="03211-115">Überprüfen Sie den Status der RetentionHold-Einstellung für das jeweilige Postfach in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="03211-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="03211-116">Führen Sie den folgenden Befehl aus, um RetentionHold für ein bestimmtes Postfach zu **Deaktivieren** :</span><span class="sxs-lookup"><span data-stu-id="03211-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="03211-117">Führen Sie nun den Assistenten für verwaltete Ordner erneut aus:</span><span class="sxs-lookup"><span data-stu-id="03211-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="03211-118">**Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, wird der Assistent für verwaltete Ordner das Postfach nicht automatisch verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="03211-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="03211-119">Weitere Informationen zu Aufbewahrungsrichtlinien im Exchange Admin Center finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="03211-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="03211-120">Aufbewahrungstags und Aufbewahrungsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="03211-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="03211-121">Anwenden einer Aufbewahrungsrichtlinie auf Postfächer</span><span class="sxs-lookup"><span data-stu-id="03211-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="03211-122">Hinzufügen oder Entfernen von Aufbewahrungstags</span><span class="sxs-lookup"><span data-stu-id="03211-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="03211-123">Vorgehensweise identifizieren des in einem Postfach gelegten Aufbewahrungs Typs</span><span class="sxs-lookup"><span data-stu-id="03211-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
