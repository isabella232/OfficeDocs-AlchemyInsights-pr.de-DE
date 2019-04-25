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
ms.openlocfilehash: ebb9037362d261b81b9b1dcafcbe461aac7f4963
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32400608"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="4b910-102">Gewähren von Benutzern Zugriff auf SharePoint und OneDrive</span><span class="sxs-lookup"><span data-stu-id="4b910-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="4b910-103">Wenn ein OneDrive oder eine SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein temporäres Dienst Problem vorliegen.</span><span class="sxs-lookup"><span data-stu-id="4b910-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="4b910-104">Überprüfen des Dienststatus-Dashboards</span><span class="sxs-lookup"><span data-stu-id="4b910-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="4b910-105">Wenn Sie möchten, dass Personen in Ihrer Organisation sich anmelden und SharePoint und OneDrive verwenden können, müssen Sie diese Konten hinzufügen und sicherstellen, dass Sie über eine Lizenz verfügen, die Ihnen Zugriff auf SharePoint und OneDrive ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="4b910-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="4b910-106">Die einfachste Möglichkeit zum Hinzufügen von Benutzern befindet sich im Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="4b910-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="4b910-107">Wechseln Sie zur [Seite aktive Benutzer im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/users), und klicken Sie dann auf **Benutzer hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="4b910-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="4b910-108">Geben Sie die Informationen für den Benutzer ein, und stellen Sie sicher, dass unter **Produktlizenzen**eine Lizenz zugewiesen und **SharePoint Online** ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="4b910-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="4b910-109">Beachten Sie, dass, wenn Sie die externe Freigabe in Ihrer Organisation zulassen, Benutzer SharePoint-und OneDrive-Inhalte für Personen außerhalb der Organisation freigeben können.</span><span class="sxs-lookup"><span data-stu-id="4b910-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="4b910-110">Sie müssen diese externen Benutzerlizenzen nicht erteilen.</span><span class="sxs-lookup"><span data-stu-id="4b910-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="4b910-111">Sie müssen auch keine Konten für Sie hinzufügen, es sei denn, die Freigabe ist auf "nur vorhandene externe Benutzer" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4b910-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="4b910-112">Wenn die Personen in diesem Fall nicht im Verzeichnis Ihrer Organisation sind, müssen Sie diese als Gastbenutzer im Azure AD Admin Center hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="4b910-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

