---
title: Automatisches Verschlüsseln bestimmter Office 365-E-Mail-Nachrichten
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509910"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="e5855-102">Automatisches Verschlüsseln bestimmter Office 365-E-Mail-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="e5855-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="e5855-103">Sie können Nachrichten, die Benutzer an bestimmte externe Personen oder Organisationen senden, automatisch verschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="e5855-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="e5855-104">Führen Sie dazu die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="e5855-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="e5855-105">Wählen Sie [im Exchange Admin Center](https://outlook.office365.com/ecp/)die Option **Nachrichtenfluss > Regeln aus.**</span><span class="sxs-lookup"><span data-stu-id="e5855-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="e5855-106">Klicken Sie **auf das Symbol Neu (+),** und klicken Sie dann auf Office **365-Nachrichtenverschlüsselung und -rechteschutz auf Nachrichten anwenden.**</span><span class="sxs-lookup"><span data-stu-id="e5855-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="e5855-107">Geben **Sie unter Name** einen Namen für die Regel ein, z. *B. Nachrichten* verschlüsseln, die an DrToniRamos@gmail.com.</span><span class="sxs-lookup"><span data-stu-id="e5855-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="e5855-108">Wählen **Sie unter Diese Regel anwenden, wenn**, die Option Empfänger > ist diese **Person** aus.</span><span class="sxs-lookup"><span data-stu-id="e5855-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="e5855-109">Wählen Sie **im** Fenster Mitglieder auswählen den Namen der Person aus, auf die die Verschlüsselungsregel angewendet werden soll, und klicken Sie dann auf **Hinzufügen.**</span><span class="sxs-lookup"><span data-stu-id="e5855-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="e5855-110">Wenn Sie mit dem Hinzufügen von Benutzern fertig sind, klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="e5855-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="e5855-111">Klicken Sie neben **dem Feld Gehen Sie wie folgt** auf Wählen Sie **eins aus.**</span><span class="sxs-lookup"><span data-stu-id="e5855-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="e5855-112">Wählen Sie **im Dropdownmenü RMS-Vorlage** die Option **Verschlüsseln** aus, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="e5855-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="e5855-113">(Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst.</span><span class="sxs-lookup"><span data-stu-id="e5855-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="e5855-114">Sie können sie jedoch hinzufügen!)</span><span class="sxs-lookup"><span data-stu-id="e5855-114">But you can add it!)</span></span>
9. <span data-ttu-id="e5855-115">Wählen Sie eine beliebige optionale Auswahl (aus einer Liste der optionalen Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber der Standardeinstellung erhalten bleiben können).</span><span class="sxs-lookup"><span data-stu-id="e5855-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="e5855-116">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="e5855-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e5855-117">Sie können diese Regel später immer wieder bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="e5855-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="e5855-118">Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="e5855-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

