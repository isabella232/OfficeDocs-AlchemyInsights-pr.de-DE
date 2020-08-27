---
title: Erstellen und Freigeben von Kalendern für öffentliche Ordner in Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: bec11baa2de7154481ec175df2466eb601b0e243
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903567"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="fb340-102">Erstellen und Freigeben von Kalendern für öffentliche Ordner in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="fb340-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="fb340-103">Kalender im öffentlichen Ordner können nur über den Outlook-Desktopclient erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="fb340-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="fb340-104">Führen Sie die folgenden Schritte aus, um Kalender für öffentliche Ordner einzurichten:</span><span class="sxs-lookup"><span data-stu-id="fb340-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="fb340-105">Stellen Sie sicher, dass die öffentlichen Ordner in Exchange Online bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="fb340-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="fb340-106">Weitere Informationen finden Sie unter [Erstellen eines Postfachs für öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="fb340-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="fb340-107">Stellen Sie sicher, dass Sie die erforderlichen Zugriffsberechtigungen zum Erstellen des öffentlichen Ordners besitzen.</span><span class="sxs-lookup"><span data-stu-id="fb340-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="fb340-108">Weitere Informationen finden Sie unter [Berechtigungen für Öffentliche Ordner für Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="fb340-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="fb340-109">Melden Sie sich beim Outlook-Desktopclient an, und stellen Sie sicher, dass Sie auf Ihre Bereitstellung öffentlicher Ordner zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="fb340-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="fb340-110">Wenn beim Zugriff auf öffentliche Ordner mit dem Outlook-Desktopclient Probleme auftreten, finden Sie entsprechende Informationen unter [Exchange Online-Benutzer können mithilfe von Outlook oder OWA keine Verbindung mit öffentlichen Ordnern herstellen](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="fb340-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="fb340-111">Erstellen Sie einen neuen Kalendertyp für öffentliche Ordner.</span><span class="sxs-lookup"><span data-stu-id="fb340-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="fb340-112">Der öffentliche Ordner wird standardmäßig für alle anderen Benutzer freigegeben.</span><span class="sxs-lookup"><span data-stu-id="fb340-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="fb340-113">Der Besitzer des öffentlichen Ordners kann die Berechtigungen im Outlook-Desktopclient ändern.</span><span class="sxs-lookup"><span data-stu-id="fb340-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="fb340-114">Weitere Informationen finden Sie unter [Berechtigungen für Öffentliche Ordner für Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="fb340-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="fb340-115">**Hinweis** Kalender für öffentliche Ordner sind für die Verwendung in der Organisation vorgesehen und können nicht im Internet veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="fb340-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="fb340-116">Verwenden Sie ein freigegebenes Postfach, wenn Sie einen Kalender im Internet veröffentlichen möchten.</span><span class="sxs-lookup"><span data-stu-id="fb340-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>