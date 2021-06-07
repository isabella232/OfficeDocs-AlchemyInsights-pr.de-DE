---
title: Laufwerkversand im Microsoft 365-Importdienst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721692"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="6f48e-102">Laufwerkversand im Microsoft 365-Importdienst</span><span class="sxs-lookup"><span data-stu-id="6f48e-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="6f48e-103">Verwenden Sie den Laufwerksversand, indem Sie die PSTs auf eine Festplatte kopieren und die Festplatte dann an Microsoft senden.</span><span class="sxs-lookup"><span data-stu-id="6f48e-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="6f48e-104">So starten Sie die Anfrage:</span><span class="sxs-lookup"><span data-stu-id="6f48e-104">To start the job:</span></span>

1. <span data-ttu-id="6f48e-105">Wählen Sie im Microsoft 365 Compliance Center unter **Informationsgovernance** die Option **Importieren**.</span><span class="sxs-lookup"><span data-stu-id="6f48e-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="6f48e-106">Wählen Sie den **Typ des Importauftrags** aus und wählen Sie dann **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="6f48e-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="6f48e-107">Wenn Sie die Schritte für diese Importoption sehen möchten, wählen Sie **Festplattenlaufwerke an einen unserer physischen Standorte versenden**.</span><span class="sxs-lookup"><span data-stu-id="6f48e-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="6f48e-108">Hier sind einige Dinge, die Sie beachten sollten:</span><span class="sxs-lookup"><span data-stu-id="6f48e-108">Here are some things to remember:</span></span>

- <span data-ttu-id="6f48e-109">Ihnen muss die Rolle für den Postfachimport/-export in Exchange Online zugewiesen sein, um PST-Dateien in Microsoft 365-Postfächer importieren zu können.</span><span class="sxs-lookup"><span data-stu-id="6f48e-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="6f48e-110">Bei PSTs mit mehr als 20 GB kann die Leistung beeinträchtigt werden.</span><span class="sxs-lookup"><span data-stu-id="6f48e-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="6f48e-111">Nur 2,5-Zoll-Festkörperlaufwerke (SSDs) oder interne 2,5-/3,5-Zoll-SATA II/III-Festplatten werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f48e-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="6f48e-112">Eine Festplatte, die PST-Dateien enthält, muss mit BitLocker verschlüsselt werden.</span><span class="sxs-lookup"><span data-stu-id="6f48e-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="6f48e-113">Die Kosten für das Importieren von PST-Dateien in Microsoft 365-Postfächer mithilfe des Laufwerkversands betragen 2 USD pro GB an Daten.</span><span class="sxs-lookup"><span data-stu-id="6f48e-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="6f48e-114">Weitere Informationen zur Verwendung der Laufwerkversandmethode für den Import von PST-Dateien finden Sie unter [Verwenden des Laufwerkversands zum Importieren der PST-Dateien Ihrer Organisation](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="6f48e-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>