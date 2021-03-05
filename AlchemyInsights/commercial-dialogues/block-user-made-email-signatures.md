---
title: Blockieren von benutzerdefinierten E-Mail-Signaturen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464618"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="6a537-102">Blockieren von benutzerdefinierten E-Mail-Signaturen</span><span class="sxs-lookup"><span data-stu-id="6a537-102">Block user-made email signatures</span></span>

<span data-ttu-id="6a537-103">Die folgende Lösung gilt nur für E-Mail-Signaturen, die in Outlook im Web erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="6a537-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="6a537-104">Sie können Signaturen in der Outlook-App nur blockieren, wenn Sie über eine lokale Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="6a537-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="6a537-105">Wählen Sie im Admin Center Admin **Center**  >  **Exchange aus.**</span><span class="sxs-lookup"><span data-stu-id="6a537-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="6a537-106">Klicken Sie **auf Berechtigungen** Outlook  >  **Web App-Richtlinien**.</span><span class="sxs-lookup"><span data-stu-id="6a537-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="6a537-107">Wählen Sie die Richtlinie aus, und klicken Sie dann auf das Stiftsymbol, um sie zu bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="6a537-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="6a537-108">Klicken Sie **auf Features**  >  **Weitere Optionen**.</span><span class="sxs-lookup"><span data-stu-id="6a537-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="6a537-109">Aktivieren **Sie unter Benutzererfahrung** das Kontrollkästchen **E-Mail-Signatur,** und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="6a537-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="6a537-110">**Wichtig:** Wenn vor dem Löschen dieses Kontrollkästchens eine Signatur hinzugefügt wurde, kann der Benutzer sie weiterhin verwenden.</span><span class="sxs-lookup"><span data-stu-id="6a537-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="6a537-111">Bitten Sie sie, sie zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="6a537-111">Ask them to remove it.</span></span>
