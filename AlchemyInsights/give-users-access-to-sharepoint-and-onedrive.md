---
title: Gewähren von Benutzern Zugriff auf SharePoint und OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36523762"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="deecd-102">Gewähren von Benutzern Zugriff auf SharePoint und OneDrive</span><span class="sxs-lookup"><span data-stu-id="deecd-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="deecd-103">Wenn eine OneDrive-oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, ist möglicherweise ein vorübergehendes Dienst Problem aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="deecd-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="deecd-104">Überprüfen des Dienst Integritäts Dashboards</span><span class="sxs-lookup"><span data-stu-id="deecd-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="deecd-105">Wenn Personen in Ihrer Organisation in der Lage sein sollen, sich anzumelden und SharePoint und OneDrive zu verwenden, müssen Sie Konten für diese hinzufügen und sicherstellen, dass Sie über eine Lizenz verfügen, die Ihnen den Zugriff auf SharePoint und OneDrive ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="deecd-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="deecd-106">Die einfachste Möglichkeit zum Hinzufügen von Benutzern finden Sie im Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="deecd-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="deecd-107">Wechseln Sie zur [Seite aktive Benutzer im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/users), und klicken Sie dann auf **Benutzer hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="deecd-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="deecd-108">Geben Sie die Informationen für den Benutzer ein, und stellen Sie sicher, dass unter **Produktlizenzen**eine Lizenz zugewiesen ist und **SharePoint Online** ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="deecd-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="deecd-109">Beachten Sie Folgendes: Wenn Sie die externe Freigabe in Ihrer Organisation zulassen, können Benutzer SharePoint-und OneDrive-Inhalte für Personen außerhalb der Organisation freigeben.</span><span class="sxs-lookup"><span data-stu-id="deecd-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="deecd-110">Sie müssen diese Lizenzen für externe Benutzer nicht erteilen.</span><span class="sxs-lookup"><span data-stu-id="deecd-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="deecd-111">Sie müssen auch keine Konten für diese hinzufügen, es sei denn, die Freigabe wird auf "nur vorhandene externe Benutzer" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="deecd-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="deecd-112">Wenn sich die Personen nicht im Verzeichnis Ihrer Organisation befinden, müssen Sie Sie in diesem Fall als Gastbenutzer im Azure AD Admin Center hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="deecd-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

