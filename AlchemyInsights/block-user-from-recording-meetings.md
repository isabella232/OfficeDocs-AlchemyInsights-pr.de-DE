---
title: Blockieren der Aufzeichnung von Besprechungen durch Benutzer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897672"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="279db-102">Blockieren der Aufzeichnung von Besprechungen durch Benutzer</span><span class="sxs-lookup"><span data-stu-id="279db-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="279db-103">Wenn Sie verhindern oder **blockieren müssen,** dass bestimmte Benutzer Teams-Besprechungen aufzeichnen, können Sie dies über die Einstellungen für Teams-Besprechungsrichtlinien tun.</span><span class="sxs-lookup"><span data-stu-id="279db-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="279db-104">Deaktivieren Sie im Microsoft Teams  Admin Center die Einstellung Cloudaufzeichnung zulassen in der Besprechungsrichtlinie, die diesem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="279db-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="279db-105">Weitere Informationen finden Sie unter [Verwalten von Besprechungsrichtlinien in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="279db-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="279db-106">Verwenden Sie die Supportdiagnose, um zu überprüfen, ob ein bestimmter Benutzer Teams-Besprechungen aufzeichnen darf oder nicht.</span><span class="sxs-lookup"><span data-stu-id="279db-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="279db-107">Führen Sie eine neue Supportabfrage aus, und geben Sie in **Diag: Besprechungsaufzeichnung ein.** Die Diagnose überprüft die Richtlinieneinstellungen für den angegebenen Benutzer und bestimmt deren Richtlinieneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="279db-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="279db-108">Denken Sie daran, dass es einige Stunden dauern kann, bis neue Richtlinieneinstellungen wirksam werden. Wenn Sie also gerade eine Änderung vorgenommen haben, warten Sie einige Stunden, bevor Sie die Diagnose erneut ausführen.</span><span class="sxs-lookup"><span data-stu-id="279db-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="279db-109">Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren der Cloudaufzeichnung.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="279db-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
