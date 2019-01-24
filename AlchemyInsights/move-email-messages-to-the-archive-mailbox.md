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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470029"
---
<span data-ttu-id="cac26-p101">Probleme bei der Archivierung von Elementen in das Archivpostfach. Stellen Sie sicher, dass Sie die folgenden Schritte ausgeführt haben:</span><span class="sxs-lookup"><span data-stu-id="cac26-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="cac26-p102">Vergewissern Sie sich, dass ein **archivieren Postfach** aktiviert wurde. Wenn dies nicht der Fall ist, verwenden Sie in [diesem Artikel](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) die Schritte aus, um das Archivpostfach aktivieren.</span><span class="sxs-lookup"><span data-stu-id="cac26-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="cac26-106">Wählen Sie in der Exchange-Verwaltungskonsole **Retention Tags** unter **Verwaltung der Richtlinientreue**, erstellen Sie ein **aufbewahrungstag** mit der Aktion **in Archiv verschieben** , enthält das gewünschte **Aufbewahrungszeitraum**.</span><span class="sxs-lookup"><span data-stu-id="cac26-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="cac26-107">Klicken Sie in der Exchange-Verwaltungskonsole wählen Sie **Aufbewahrungsrichtlinien**, erstellen Sie eine **Aufbewahrungsrichtlinie** , und fügen Sie Ihrer aufbewahrungstag **in Archiv verschieben** dieser Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="cac26-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="cac26-p103">Sie [weisen die Aufbewahrungsrichtlinie](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Postfach für den betreffenden Benutzer. Die gleiche Richtlinie wird auf **primäre** und **das Archivpostfach** angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="cac26-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="cac26-p104">Das Postfach des Benutzers sollte jetzt eine Archivrichtlinie Elemente in das Archivpostfach verschieben. Möglicherweise erforderlich sind, um zu erzwingen, dass die verwaltete Ordner-Assistent (mehrstufiger Authentifizierung das) ausführen und die neuen Einstellungen auf das Postfach des Benutzers angewendet werden. Führen Sie den folgenden Befehl während [EXO PowerShell verbunden](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:</span><span class="sxs-lookup"><span data-stu-id="cac26-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="cac26-113">Möchten Sie weitere Informationen zum Einrichten einer Richtlinie für den archivieren, finden Sie unter [Set up ein Archiv und Löschung Richtlinie für Postfächer](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="cac26-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

