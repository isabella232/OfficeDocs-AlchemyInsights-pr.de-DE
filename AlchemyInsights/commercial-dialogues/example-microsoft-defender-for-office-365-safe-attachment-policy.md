---
title: Beispiel für microsoft defender for Office 365 Safe Attachment policy
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
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736751"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="af179-102">Beispiel für microsoft defender for Office 365 Safe Attachment policy</span><span class="sxs-lookup"><span data-stu-id="af179-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="af179-103">Mit diesen Einstellungen wird eine Richtlinie namens *Keine* Verzögerungen aktiviert, die Nachrichten sofort übermittelt und anlagen nach dem Scannen erneut angibt:</span><span class="sxs-lookup"><span data-stu-id="af179-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="af179-104">**Name**: Keine Verzögerungen</span><span class="sxs-lookup"><span data-stu-id="af179-104">**Name**: No delays</span></span>
- <span data-ttu-id="af179-105">**Beschreibung**: Übermittelt Nachrichten sofort und legt Anlagen nach dem Scannen erneut an.</span><span class="sxs-lookup"><span data-stu-id="af179-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="af179-106">**Antwort**: Wählen Sie die **Option Dynamische Zustellung** aus.</span><span class="sxs-lookup"><span data-stu-id="af179-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="af179-107">Weitere Informationen finden Sie unter [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="af179-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="af179-108">**Abschnitt** Umleitungsanlage: Wählen Sie die Option Umleitung aktivieren **aus,** und geben Sie dann die E-Mail-Adresse Ihres globalen Microsoft 365-Administrators, Sicherheitsadministrators oder Sicherheitsanalysten ein, der schädliche Anlagen untersuchen wird.</span><span class="sxs-lookup"><span data-stu-id="af179-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="af179-109">**Abschnitt Angewendet auf:** Wählen Sie **Die Empfängerdomäne ist**, und wählen Sie dann Ihre Domäne aus.</span><span class="sxs-lookup"><span data-stu-id="af179-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="af179-110">Wählen **Sie Hinzufügen** aus, und wählen Sie dann OK **aus.**</span><span class="sxs-lookup"><span data-stu-id="af179-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="af179-111">Nachdem Sie fertig sind, wählen Sie **Speichern aus.**</span><span class="sxs-lookup"><span data-stu-id="af179-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="af179-112">Weitere Informationen finden Sie unter [Sichere Anlagen in Microsoft Defender für Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="af179-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
