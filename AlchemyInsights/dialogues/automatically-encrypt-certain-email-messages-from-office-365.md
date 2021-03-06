---
title: Automatisches Verschlüsseln bestimmter E-Mail-Nachrichten aus Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509916"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="ff203-102">Automatisches Verschlüsseln bestimmter E-Mail-Nachrichten aus Office 365</span><span class="sxs-lookup"><span data-stu-id="ff203-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="ff203-103">Wählen Sie [im Exchange Admin Center](https://outlook.office365.com/ecp/)die Option **Nachrichtenfluss > Regeln aus.**</span><span class="sxs-lookup"><span data-stu-id="ff203-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="ff203-104">Klicken Sie **auf das Symbol Neu (+),** und klicken Sie dann auf Office **365-Nachrichtenverschlüsselung und -rechteschutz auf Nachrichten anwenden.**</span><span class="sxs-lookup"><span data-stu-id="ff203-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="ff203-105">Geben Sie unter **Name** einen Namen für die Regel ein, z. *B. Alle Nachrichten verschlüsseln.*</span><span class="sxs-lookup"><span data-stu-id="ff203-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="ff203-106">Wählen **Sie unter Diese Regel anwenden, wenn** die Option **[Auf alle Nachrichten anwenden] aus.**</span><span class="sxs-lookup"><span data-stu-id="ff203-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="ff203-107">Klicken Sie neben **dem Feld Gehen Sie wie folgt** auf Wählen Sie **eins aus.**</span><span class="sxs-lookup"><span data-stu-id="ff203-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="ff203-108">Wählen Sie **im Dropdownmenü RMS-Vorlage** die Option **Verschlüsseln** aus, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="ff203-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="ff203-109">(Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst.</span><span class="sxs-lookup"><span data-stu-id="ff203-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="ff203-110">Sie können sie jedoch hinzufügen!)</span><span class="sxs-lookup"><span data-stu-id="ff203-110">But you can add it!)</span></span>
7. <span data-ttu-id="ff203-111">Aktivieren Sie das Kontrollkästchen Diese **Regel mit Schweregrad überwachen,** und wählen Sie dann die gewünschte Ebene aus.</span><span class="sxs-lookup"><span data-stu-id="ff203-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="ff203-112">Wenn Ihr Unternehmen vertragliche Verpflichtungen zum Senden aller verschlüsselten E-Mails hat, empfiehlt es sich, die Stufe auf **Hoch zu setzen.**</span><span class="sxs-lookup"><span data-stu-id="ff203-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="ff203-113">Klicken **Sie unter Modell für diese Regel auswählen** auf **Erzwingen**.</span><span class="sxs-lookup"><span data-stu-id="ff203-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="ff203-114">Wählen Sie eine beliebige optionale Auswahl (aus einer Liste der optionalen Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber der Standardeinstellung erhalten bleiben können).</span><span class="sxs-lookup"><span data-stu-id="ff203-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="ff203-115">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="ff203-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ff203-116">Sie können diese Regel später immer wieder bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="ff203-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="ff203-117">Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="ff203-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

