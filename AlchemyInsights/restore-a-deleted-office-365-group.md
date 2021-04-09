---
title: Wiederherstellen einer gelöschten Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645130"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="c7776-102">Wiederherstellen einer gelöschten Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="c7776-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="c7776-103">Sie können eine gelöschte Microsoft 365-Gruppe oder Microsoft Teams innerhalb von 30 Tagen nach dem Löschen wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="c7776-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="c7776-104">Wechseln Sie zum [Microsoft 365 Admin Center,](https://aka.ms/RestoreDeletedGroup) um sich bei einer Liste der gelöschten Gruppen und Teams zu melden.</span><span class="sxs-lookup"><span data-stu-id="c7776-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="c7776-105">**Hinweis:** Melden Sie sich mit dem Konto an, das entweder dem Mandantenadministrator oder der Gruppenadministratorrolle zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c7776-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="c7776-106">Wählen Sie die gelöschte Microsoft 365-Gruppe/Teams aus, die wiederhergestellt werden soll, und klicken Sie auf **Wiederherstellungsgruppe**.</span><span class="sxs-lookup"><span data-stu-id="c7776-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="c7776-107">Wenn die Gruppe aufgrund einer in Konflikt enden SMTP-Adresse nicht wiederhergestellt werden kann, verwenden Sie den folgenden Befehl, um das Objekt zu finden, das einen Konflikt verursacht, und entfernen Sie die SMTP-Adresse:</span><span class="sxs-lookup"><span data-stu-id="c7776-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="c7776-108">**Hinweis:** In einigen Fällen kann es bis zu 24 Stunden dauern, bis die Gruppe und alle ihre Daten wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="c7776-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="c7776-109">Weitere Informationen oder Informationen zum Wiederherstellen von Gruppen mithilfe von PowerShell finden Sie unter [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="c7776-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>