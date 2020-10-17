---
title: Vorgehensweise zum Erweitern des Speichers in OneDrive für Unternehmen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/16/2020
ms.locfileid: "48489006"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="0f08f-102">Vorgehensweise zum Erweitern des Speichers in OneDrive für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="0f08f-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="0f08f-103">So ändern Sie den Standardspeicher für neue und vorhandene OneDrive-Benutzer:</span><span class="sxs-lookup"><span data-stu-id="0f08f-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="0f08f-104">Wechseln Sie zur [Seite Speicher des OneDrive Admin Center](https://admin.onedrive.com/?v=StorageSettings), geben Sie einen neuen Betrag in GB ein, und wählen Sie dann **Speichern**aus.</span><span class="sxs-lookup"><span data-stu-id="0f08f-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="0f08f-105">Diese Speicherplatz Einstellung gilt für alle Benutzer, für die Sie keine bestimmten Speichergrenzwerte festgelegt haben.</span><span class="sxs-lookup"><span data-stu-id="0f08f-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="0f08f-106">Verwenden Sie Microsoft PowerShell, um den Speicherplatz für bestimmte Benutzer zu ändern.</span><span class="sxs-lookup"><span data-stu-id="0f08f-106">To change the storage space for specific users, use Microsoft PowerShell.</span></span> <span data-ttu-id="0f08f-107">Informationen zur Vorgehensweise finden Sie unter [Ändern des OneDrive-Speicherplatzes Ihrer Benutzer mithilfe von PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span><span class="sxs-lookup"><span data-stu-id="0f08f-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="0f08f-108">**Hinweis**: Es sieht so aus, dass Sie keinen Plan haben, der unbegrenzten Speicher enthält.</span><span class="sxs-lookup"><span data-stu-id="0f08f-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="0f08f-109">Informationen zum Speicherplatz, der mit den einzelnen Plänen geliefert wird, finden Sie unter [OneDrive für Unternehmen-Dienstbeschreibung](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="0f08f-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="0f08f-110">Um den Speicherplatz in OneDrive für Unternehmen zu verbessern, wählen Sie ein Abonnement aus, das entweder **OneDrive für Unternehmen Plan 2** oder **Office 365 E3**enthält.</span><span class="sxs-lookup"><span data-stu-id="0f08f-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="0f08f-111">Zum Ändern der Pläne wechseln Sie im Admin Center zur Seite **Fakturierung** \> [ihrer Produkte](https://go.microsoft.com/fwlink/p/?linkid=842054) , wählen Sie das zu ändernde Abonnement aus, und wählen Sie dann **für Ihre Organisation empfohlene Upgrades anzeigen**aus.</span><span class="sxs-lookup"><span data-stu-id="0f08f-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="0f08f-112">Weitere Informationen zum Ändern von Plänen und OneDrive für Unternehmen Speicher finden Sie unter [Upgrade auf einen anderen Plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) und die [OneDrive für Unternehmen-Dienstbeschreibung](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="0f08f-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>