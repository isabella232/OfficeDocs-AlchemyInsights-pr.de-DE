---
title: Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736776"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="fbf67-102">Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach</span><span class="sxs-lookup"><span data-stu-id="fbf67-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="fbf67-103">So richten Sie eine Richtlinie ein, um die alten E-Mails eines Benutzers automatisch in das Archivpostfach zu verschieben:</span><span class="sxs-lookup"><span data-stu-id="fbf67-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="fbf67-104">Wechseln Sie [**zu Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data Governance Archive, um zu überprüfen, ob ein Archivpostfach für den Benutzer aktiviert  >    >   wurde.</span><span class="sxs-lookup"><span data-stu-id="fbf67-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="fbf67-105">Falls nicht, klicken Sie im **Warnfeld** auf Aktivieren **und** dann auf Ja.</span><span class="sxs-lookup"><span data-stu-id="fbf67-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="fbf67-106">Wechseln Sie [**zu Exchange Admin Center > Compliance management > Aufbewahrungstags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="fbf67-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="fbf67-107">Wählen Sie das Symbol + und dann **automatisch auf das gesamte Postfach anwenden aus.**</span><span class="sxs-lookup"><span data-stu-id="fbf67-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="fbf67-108">Weisen Sie dem Aufbewahrungstag einen Namen zu, und wählen **Sie In Archiv verschieben aus.**</span><span class="sxs-lookup"><span data-stu-id="fbf67-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="fbf67-109">Geben Sie für den Aufbewahrungszeitraum die zeit ein, die Sie möchten, z. B. 90 Tage.</span><span class="sxs-lookup"><span data-stu-id="fbf67-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="fbf67-110">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="fbf67-110">Click **Save**.</span></span>
5. <span data-ttu-id="fbf67-111">Erstellen Sie nun eine Aufbewahrungsrichtlinie: Wählen Sie **Aufbewahrungsrichtlinien** aus, wählen Sie das Symbol aus, um eine neue Richtlinie hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="fbf67-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="fbf67-112">Weisen Sie der Aufbewahrungsrichtlinie einen Namen zu, und klicken Sie dann auf und scrollen Sie, um das gerade erstellte Aufbewahrungstag zu finden und hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="fbf67-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="fbf67-113">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="fbf67-113">Click **Save**.</span></span>
7. <span data-ttu-id="fbf67-114">Wenden Sie schließlich die Aufbewahrungsrichtlinie auf das Postfach des Benutzers an: Wechseln Sie noch im Exchange Admin Center zu  >  **Empfängerpostfächer**.</span><span class="sxs-lookup"><span data-stu-id="fbf67-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="fbf67-115">Wählen Sie alle Benutzer aus, auf die Sie die Richtlinie anwenden möchten, und klicken Sie dann **auf Bearbeiten** (das Stiftsymbol).</span><span class="sxs-lookup"><span data-stu-id="fbf67-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="fbf67-116">Klicken Sie im Dialogfeld auf **Postfachfeatures**.</span><span class="sxs-lookup"><span data-stu-id="fbf67-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="fbf67-117">Wenden **Sie unter** Aufbewahrungsrichtlinie die Richtlinie an, die Sie gerade > Speichern erstellt **haben.**</span><span class="sxs-lookup"><span data-stu-id="fbf67-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="fbf67-118">Anweisungen zum Anwenden der Richtlinie auf alle Benutzer finden Sie unter [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="fbf67-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
