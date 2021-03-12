---
title: Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737000"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="a4528-102">Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation</span><span class="sxs-lookup"><span data-stu-id="a4528-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="a4528-103">Gehen Sie wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="a4528-103">Follow these steps:</span></span>

1. <span data-ttu-id="a4528-104">Wenn Sie kein globaler Administrator sind, muss Ihr Konto zur Rollengruppe **eDiscovery-Manager** oder zur Verwaltungsrolle **"Compliancesuche"** hinzugefügt werden, um nach Nachrichten zu suchen.</span><span class="sxs-lookup"><span data-stu-id="a4528-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="a4528-105">Zum Löschen von Nachrichten müssen Sie  der Rollengruppe Organisationsverwaltung oder der Verwaltungsrolle Suchen und Löschen **beitreten.**</span><span class="sxs-lookup"><span data-stu-id="a4528-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="a4528-106">Berechtigungen für diese Rollen werden im [Security & Compliance Center zugewiesen.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="a4528-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="a4528-107">[Erstellen Sie eine Inhaltssuche,](https://docs.microsoft.com/office365/securitycompliance/content-search) um die zu löschende Nachricht zu finden.</span><span class="sxs-lookup"><span data-stu-id="a4528-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="a4528-108">[Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a4528-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="a4528-109">Wenn Sie MFA verwenden, lesen Sie die folgenden Anweisungen: Verbinden mit Security [& Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="a4528-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="a4528-110">Nachricht löschen: Führen Sie das `New-ComplianceSearchAction` Cmdlet aus, um die Nachricht zu löschen.</span><span class="sxs-lookup"><span data-stu-id="a4528-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="a4528-111">Gelöschte Nachrichten werden in den Ordner "Wiederherstellbare Elemente" eines Benutzers verschoben.</span><span class="sxs-lookup"><span data-stu-id="a4528-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="a4528-112">Ein Beispielbefehl finden Sie unter [Schritt 3: Löschen der Nachricht.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="a4528-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
