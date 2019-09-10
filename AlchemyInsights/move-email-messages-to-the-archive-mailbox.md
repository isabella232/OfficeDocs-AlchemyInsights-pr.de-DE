---
title: E-Mail-Nachrichten in das Archivpostfach migrieren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822161"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="76417-102">E-Mail-Nachricht in das Archivpostfach migrieren</span><span class="sxs-lookup"><span data-stu-id="76417-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="76417-103">Stellen Sie sicher, dass ein **Archivpostfach** aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="76417-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="76417-104">Wenn dies nicht der Fall ist, verwenden Sie die Schritte in [diesem Artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , um das Archivpostfach zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76417-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="76417-105">Um Nachrichten automatisch in das Archivpostfach zu archivieren, muss ein Aufbewahrungs mit der Aktion **in Archiv** verlegen auf **automatisch auf gesamtes Postfach (Standard) angewendet**werden.</span><span class="sxs-lookup"><span data-stu-id="76417-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="76417-106">Verwenden Sie die Schritte hier, um das Tag: [Archive default-Tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="76417-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="76417-107">Fügen Sie als nächstes das **Archiv** -Tag zu ihrer Aufbewahrungsrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="76417-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="76417-108">Wählen Sie in der Exchange-Verwaltungskonsole die Option **Aufbewahrungsrichtlinien** #a0 fügen Sie der Richtlinie #a1 **Speichern**das **Element zum Archivieren** hinzu.</span><span class="sxs-lookup"><span data-stu-id="76417-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="76417-109">[Weisen Sie die Aufbewahrungsrichtlinie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nun dem Postfach des jeweiligen Benutzers zu.</span><span class="sxs-lookup"><span data-stu-id="76417-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="76417-110">Dieselbe Richtlinie wird sowohl auf das **primäre** als auch auf das **Archiv** Postfach angewendet.</span><span class="sxs-lookup"><span data-stu-id="76417-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="76417-111">Es kann erforderlich sein, die Ausführung des Assistenten für verwaltete Ordner (MFA) zu erzwingen und die neuen Einstellungen auf das Postfach des Benutzers anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="76417-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="76417-112">Führen Sie den folgenden Befehl aus, während eine [Verbindung mit Exo PowerShell hergestellt](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) wurde, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:</span><span class="sxs-lookup"><span data-stu-id="76417-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="76417-113">Start-ManagedFolderAssistant-Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="76417-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="76417-114">Weitere Informationen zum Einrichten einer Archivrichtlinie finden Sie unter [Einrichten einer Archiv-und Löschrichtlinie für Postfächer](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="76417-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  