---
title: Öffentliche Ordner ausblenden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294642"
---
# <a name="hide-public-folders"></a><span data-ttu-id="d1cc9-102">Öffentliche Ordner ausblenden</span><span class="sxs-lookup"><span data-stu-id="d1cc9-102">Hide public folders</span></span>

<span data-ttu-id="d1cc9-103">**So blenden Sie die gesamte öffentliche Ordnerstruktur aus**:</span><span class="sxs-lookup"><span data-stu-id="d1cc9-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="d1cc9-104">Verwenden Sie die Schritte in [diesem](https://aka.ms/ControlPF) Artikel, um die gesamte öffentliche Ordnerstruktur vor ausgewählten oder allen Benutzern zu verbergen.</span><span class="sxs-lookup"><span data-stu-id="d1cc9-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="d1cc9-105">**So blenden Sie einen bestimmten öffentlichen Ordner aus**:</span><span class="sxs-lookup"><span data-stu-id="d1cc9-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="d1cc9-106">Hinzufügen von Berechtigungen für Benutzer, die auf den öffentlichen Ordner zugreifen müssen</span><span class="sxs-lookup"><span data-stu-id="d1cc9-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="d1cc9-107">Entfernen Sie den Benutzer **Standard** aus der **Berechtigungsliste**:</span><span class="sxs-lookup"><span data-stu-id="d1cc9-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
