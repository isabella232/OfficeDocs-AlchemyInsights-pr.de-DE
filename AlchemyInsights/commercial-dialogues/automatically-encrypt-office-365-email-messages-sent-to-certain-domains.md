---
title: Automatische Verschlüsselung von Office 365-E-Mail-Nachrichten, die an bestimmte Domänen gesendet werden
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736783"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="7c8ec-102">Automatische Verschlüsselung von Office 365-E-Mail-Nachrichten, die an bestimmte Domänen gesendet werden</span><span class="sxs-lookup"><span data-stu-id="7c8ec-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="7c8ec-103">Wählen Sie [im Exchange Admin Center](https://outlook.office365.com/ecp/)die Option **Nachrichtenfluss > Regeln aus.**</span><span class="sxs-lookup"><span data-stu-id="7c8ec-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="7c8ec-104">Klicken Sie **auf das Symbol Neu (+),** und klicken Sie dann auf Office **365-Nachrichtenverschlüsselung und -rechteschutz auf Nachrichten anwenden.**</span><span class="sxs-lookup"><span data-stu-id="7c8ec-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="7c8ec-105">Geben Sie unter **Name** einen Namen für die Regel ein, z. B. Nachrichten *verschlüsseln, die an contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="7c8ec-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="7c8ec-106">Wählen **Sie unter Diese Regel anwenden, wenn**, die Option Empfänger > Domäne **ist** aus.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="7c8ec-107">Geben Sie den Namen der Domäne ein, z. **B. contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="7c8ec-108">Klicken Sie **auf das Symbol Hinzufügen (+),** und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="7c8ec-109">Klicken Sie neben **dem Feld Gehen Sie wie folgt** auf Wählen Sie **eins aus.**</span><span class="sxs-lookup"><span data-stu-id="7c8ec-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="7c8ec-110">Wählen Sie **im Dropdownmenü RMS-Vorlage** die Option **Verschlüsseln** aus, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="7c8ec-111">(Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="7c8ec-112">Sie können sie jedoch hinzufügen!)</span><span class="sxs-lookup"><span data-stu-id="7c8ec-112">But you can add it!)</span></span>
9. <span data-ttu-id="7c8ec-113">Wählen Sie eine beliebige optionale Auswahl (aus einer Liste der optionalen Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber der Standardeinstellung erhalten bleiben können).</span><span class="sxs-lookup"><span data-stu-id="7c8ec-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="7c8ec-114">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7c8ec-115">Sie können diese Regel später immer wieder bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="7c8ec-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="7c8ec-116">Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="7c8ec-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>