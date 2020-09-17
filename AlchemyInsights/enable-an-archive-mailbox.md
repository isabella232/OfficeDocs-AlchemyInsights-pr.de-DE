---
title: Aktivieren eines Archivpostfachs
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811704"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="abe5c-102">Aktivieren eines Archivpostfachs</span><span class="sxs-lookup"><span data-stu-id="abe5c-102">Enable an archive mailbox</span></span>

<span data-ttu-id="abe5c-103">Wenn Sie möchten, dass automatisierte Prüfungen ausgeführt werden, um sicherzustellen, dass ein Archivpostfach konfiguriert werden kann, wählen Sie die Schaltfläche Zurück <--oben auf dieser Seite aus, und geben Sie dann die e-Mail-Adresse des Kontos ein.</span><span class="sxs-lookup"><span data-stu-id="abe5c-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="abe5c-104">Archivpostfächer in Microsoft 365 (auch als *Online Archive* oder *in-Place-Archive*bezeichnet) bieten Benutzern zusätzlichen e-Mail-Speicher.</span><span class="sxs-lookup"><span data-stu-id="abe5c-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="abe5c-105">Benutzer können Elemente in Ihr Archivpostfach verschieben oder kopieren, und Administratoren können eine Archivrichtlinie erstellen, mit der Elemente automatisch in Archivpostfächer verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="abe5c-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="abe5c-106">Hier erfahren Sie, wie Sie ein Archivpostfach erstellen:</span><span class="sxs-lookup"><span data-stu-id="abe5c-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="abe5c-107">Wechseln Sie zu [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="abe5c-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="abe5c-108">Melden Sie sich bei Microsoft 365 mit Ihrem Administratorkonto an.</span><span class="sxs-lookup"><span data-stu-id="abe5c-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="abe5c-109">Wählen Sie im linken Bereich des Security &amp; Compliance Centers die Option **Information Governance** \> **Archive**aus.</span><span class="sxs-lookup"><span data-stu-id="abe5c-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="abe5c-110">Wählen Sie den Benutzer aus, dessen Archivpostfach Sie aktivieren möchten.</span><span class="sxs-lookup"><span data-stu-id="abe5c-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="abe5c-111">Klicken Sie im Detailbereich auf der rechten Seite auf **aktivieren** , und klicken Sie dann in der Warnmeldung auf **Ja** , um das Archivpostfach zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="abe5c-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="abe5c-112">Sie können Archivpostfächer auch Massen aktivieren, indem Sie mehrere Benutzer auswählen (mithilfe der **UMSCHALT** -oder **STRG** -Taste) und dann im Detailbereich auf **aktivieren** klicken.</span><span class="sxs-lookup"><span data-stu-id="abe5c-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="abe5c-113">Freigegebene Postfächer</span><span class="sxs-lookup"><span data-stu-id="abe5c-113">Shared mailboxes</span></span>

<span data-ttu-id="abe5c-114">Um das Archiv für ein freigegebenes Postfach zu aktivieren, ist eine Exchange Online Plan 2-Lizenz oder eine Exchange Onlineplan 1-Lizenz mit einer Exchange Online-Archivierungslizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="abe5c-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="abe5c-115">So aktivieren Sie das Archiv für ein freigegebenes Postfach:</span><span class="sxs-lookup"><span data-stu-id="abe5c-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="abe5c-116">Wechseln Sie zur [Exchange-Verwaltungskonsole](https://outlook.office365.com/ecp) , und melden Sie sich mit Ihrem Administratorkonto an.</span><span class="sxs-lookup"><span data-stu-id="abe5c-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="abe5c-117">Wechseln Sie zu **Empfänger**  >  **freigegeben**.</span><span class="sxs-lookup"><span data-stu-id="abe5c-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="abe5c-118">Wählen Sie das freigegebene Postfach aus.</span><span class="sxs-lookup"><span data-stu-id="abe5c-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="abe5c-119">Klicken Sie im Detailbereich auf der rechten Seite unter **in-Place Archive**auf **aktivieren**, und klicken Sie dann auf **Ja** , um das Archivpostfach zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="abe5c-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="abe5c-120">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="abe5c-120">For more information, see:</span></span>
  
- [<span data-ttu-id="abe5c-121">Aktivieren von Archivpostfächern</span><span class="sxs-lookup"><span data-stu-id="abe5c-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="abe5c-122">Einrichten einer Archivierungs- und Löschrichtlinie</span><span class="sxs-lookup"><span data-stu-id="abe5c-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
