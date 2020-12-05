---
title: Vorgehensweise, wenn Azure-Funktionen in Microsoft Edge nicht ordnungsgemäß funktionieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576485"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="47c05-102">Vorgehensweise, wenn Azure-Funktionen in Microsoft Edge nicht ordnungsgemäß funktionieren</span><span class="sxs-lookup"><span data-stu-id="47c05-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="47c05-103">Microsoft Edge hat [bekannte Probleme](https://go.microsoft.com/fwlink/?linkid=2140608) im Zusammenhang mit Sicherheitszonen und wirkt sich möglicherweise darauf aus, wie Azure-Benutzer sich bei Windows Admin Center anmelden.</span><span class="sxs-lookup"><span data-stu-id="47c05-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="47c05-104">Wenn Sie bei der Verwendung von Azure-Funktionen mit Microsoft Edge Probleme haben, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="47c05-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="47c05-105">Suchen Sie im **Startmenü** nach **Internet Optionen** , und wählen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="47c05-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="47c05-106">Wechseln Sie im Dialogfeld **Internet Eigenschaften** zur Registerkarte **Sicherheit** .</span><span class="sxs-lookup"><span data-stu-id="47c05-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="47c05-107">Wählen Sie die Zone **Vertrauenswürdige Sites** aus, und wählen Sie dann die Schaltfläche **Sites** aus.</span><span class="sxs-lookup"><span data-stu-id="47c05-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="47c05-108">Fügen Sie im Dialogfeld **vertrauenswürdige Websites** die Gateway-URL sowie [https://login.microsoftonline.com](https://login.microsoftonline.com) und ein [https://login.live.com](https://login.live.com) , und wählen Sie dann **Schließen** aus.</span><span class="sxs-lookup"><span data-stu-id="47c05-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="47c05-109">Wechseln Sie im Dialogfeld **Internet Eigenschaften** zur Registerkarte **Datenschutz** .</span><span class="sxs-lookup"><span data-stu-id="47c05-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="47c05-110">Wählen Sie im Abschnitt **Popupblocker** die Option **Einstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="47c05-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="47c05-111">Fügen Sie im daraufhin geöffneten Dialogfeld die Gateway-URL sowie und ein [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) , und wählen Sie dann **Schließen** aus.</span><span class="sxs-lookup"><span data-stu-id="47c05-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
