---
title: Aufbewahrungsrichtlinien im Exchange Admin Center funktionieren nicht
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740509"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e619b-102">Aufbewahrungsrichtlinien im Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="e619b-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="e619b-103">Wenn Sie möchten, dass automatisierte Prüfungen für die unten aufgeführten Einstellungen ausgeführt werden, wählen Sie die Schaltfläche Zurück <--oben auf dieser Seite aus, und geben Sie dann die e-Mail-Adresse des Benutzers ein, der Probleme mit Aufbewahrungsrichtlinien hat.</span><span class="sxs-lookup"><span data-stu-id="e619b-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="e619b-104">**Problem:** Neu erstellte oder aktualisierte Aufbewahrungsrichtlinien im Exchange Admin Center gelten nicht für Postfächer oder Elemente werden nicht in das Archivpostfach verschoben oder gelöscht.</span><span class="sxs-lookup"><span data-stu-id="e619b-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e619b-105">**Ursachen:**</span><span class="sxs-lookup"><span data-stu-id="e619b-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="e619b-106">Dies kann daran liegen, dass der **Assistent für verwaltete Ordner** das Postfach des Benutzers nicht verarbeitet hat.</span><span class="sxs-lookup"><span data-stu-id="e619b-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="e619b-107">Der Assistent für verwaltete Ordner versucht, jedes Postfach in ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="e619b-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="e619b-108">Wenn Sie ein Aufbewahrungs ändern oder eine andere Aufbewahrungsrichtlinie auf ein Postfach anwenden, können Sie warten, bis die Unterstützung für verwaltete Ordner das Postfach verarbeitet, oder Sie können das Cmdlet Start-ManagedFolderAssistant ausführen, um den Assistenten für verwaltete Ordner zu starten, um ein bestimmtes Postfach zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="e619b-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="e619b-109">Das Ausführen dieses Cmdlets ist hilfreich zum Testen oder Problembehandlung einer Aufbewahrungsrichtlinie oder von Aufbewahrungstags Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="e619b-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="e619b-110">Weitere Informationen finden Sie unter [Ausführen des Assistenten für verwaltete Ordner](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e619b-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e619b-111">**Lösung:** Führen Sie den folgenden Befehl aus, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:</span><span class="sxs-lookup"><span data-stu-id="e619b-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e619b-112">Dies kann auch auftreten, wenn **RetentionHold** für das Postfach **aktiviert** wurde.</span><span class="sxs-lookup"><span data-stu-id="e619b-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="e619b-113">Wenn das Postfach auf einem RetentionHold gespeichert wurde, wird die Aufbewahrungsrichtlinie für das Postfach während dieser Zeit nicht verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="e619b-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="e619b-114">Weitere Informaton für die RetentionHold-Einstellung finden Sie unter: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e619b-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e619b-115">**Lösung**</span><span class="sxs-lookup"><span data-stu-id="e619b-115">**Solution:**</span></span>
    
  - <span data-ttu-id="e619b-116">Überprüfen Sie den Status der RetentionHold-Einstellung für das jeweilige Postfach in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="e619b-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e619b-117">Führen Sie den folgenden Befehl aus, um RetentionHold für ein bestimmtes Postfach zu **Deaktivieren** :</span><span class="sxs-lookup"><span data-stu-id="e619b-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e619b-118">Führen Sie nun den Assistenten für verwaltete Ordner erneut aus:</span><span class="sxs-lookup"><span data-stu-id="e619b-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e619b-119">**Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, wird der Assistent für verwaltete Ordner das Postfach nicht automatisch verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="e619b-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="e619b-120">Weitere Informationen zu Aufbewahrungsrichtlinien im Exchange Admin Center finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="e619b-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="e619b-121">Aufbewahrungstags und Aufbewahrungsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="e619b-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="e619b-122">Anwenden einer Aufbewahrungsrichtlinie auf Postfächer</span><span class="sxs-lookup"><span data-stu-id="e619b-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="e619b-123">Hinzufügen oder Entfernen von Aufbewahrungstags</span><span class="sxs-lookup"><span data-stu-id="e619b-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="e619b-124">Identifizieren des auf ein Postfach angewandten Aufbewahrungstyps</span><span class="sxs-lookup"><span data-stu-id="e619b-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
