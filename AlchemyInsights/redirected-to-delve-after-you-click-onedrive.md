---
title: OneDrive for Business Web OneDrive-Umleitungen zu Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799988"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="ab9e2-102">Umgeleitet zu Delve, nachdem Sie auf OneDrive geklickt haben</span><span class="sxs-lookup"><span data-stu-id="ab9e2-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="ab9e2-103">Weitere Informationen finden Sie im [ausführlichen Handbuch zur Problembehandlung.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ab9e2-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="ab9e2-104">Um dieses Problem zu beheben, muss der Administrator Benutzern das Recht zum Erstellen ihrer Website "Meine Websites" erteilen.</span><span class="sxs-lookup"><span data-stu-id="ab9e2-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="ab9e2-105">Dies liegt daran, dass die OneDrive for #A0 auf "Meine Websites" erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="ab9e2-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="ab9e2-106">Führen Sie die folgenden Schritte aus, um dieses Recht zu gewähren:</span><span class="sxs-lookup"><span data-stu-id="ab9e2-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="ab9e2-107">Klicken Sie im SharePoint Admin Center auf **Benutzerprofile**.</span><span class="sxs-lookup"><span data-stu-id="ab9e2-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="ab9e2-108">Klicken Sie **im Abschnitt Personen** auf **Benutzerberechtigungen verwalten.**</span><span class="sxs-lookup"><span data-stu-id="ab9e2-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="ab9e2-109">Fügen Sie Benutzer hinzu, die Berechtigungen zum Erstellen ihrer Website "Meine Websites" benötigen.</span><span class="sxs-lookup"><span data-stu-id="ab9e2-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="ab9e2-110">Standardmäßig ist diese Einstellung auf Jeder außer externen **Benutzern festgelegt.**</span><span class="sxs-lookup"><span data-stu-id="ab9e2-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="ab9e2-111">Nachdem Sie den Benutzer, die Benutzer oder die Gruppe hinzugefügt haben, stellen Sie sicher, dass der hinzugefügte Benutzer, benutzer oder die Gruppe ausgewählt ist, scrollen Sie zum Abschnitt Berechtigungen, und aktivieren Sie dann das Kontrollkästchen neben Persönliche Website erstellen (erforderlich für persönlichen **Speicher, Newsfeed** und gefolgten Inhalt). </span><span class="sxs-lookup"><span data-stu-id="ab9e2-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="ab9e2-112">Klicken **Sie auf OK,** und navigieren Sie dann zur OneDrive-Seite, um die Website zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ab9e2-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
