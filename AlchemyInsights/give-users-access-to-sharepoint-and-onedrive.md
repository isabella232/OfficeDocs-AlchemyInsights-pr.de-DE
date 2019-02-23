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
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d29764266f44aee5f8f8e2c93ad67b2a33c6f417
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/22/2019
ms.locfileid: "30209736"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="1d870-102">Gewähren von Benutzern Zugriff auf SharePoint und OneDrive</span><span class="sxs-lookup"><span data-stu-id="1d870-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="1d870-p101">Wenn ein OneDrive oder eine SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein temporäres Dienst Problem vorliegen. [Überprüfen des Dienststatus](https://portal.office.com/adminportal/home#/servicehealth) -Dashboards</span><span class="sxs-lookup"><span data-stu-id="1d870-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="1d870-p102">Wenn Sie möchten, dass Personen in Ihrer Organisation sich anmelden und SharePoint und OneDrive verwenden können, müssen Sie diese Konten hinzufügen und sicherstellen, dass Sie über eine Lizenz verfügen, die Ihnen Zugriff auf SharePoint und OneDrive ermöglicht. Die einfachste Möglichkeit zum Hinzufügen von Benutzern befindet sich im Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="1d870-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="1d870-107">Wechseln Sie zur [Seite aktive Benutzer im Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/users), und klicken Sie dann auf **Benutzer hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="1d870-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="1d870-108">Geben Sie die Informationen für den Benutzer ein, und stellen Sie sicher, dass unter **Produktlizenzen**eine Lizenz zugewiesen und **SharePoint Online** ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="1d870-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="1d870-p103">Beachten Sie, dass, wenn Sie die externe Freigabe in Ihrer Organisation zulassen, Benutzer SharePoint-und OneDrive-Inhalte für Personen außerhalb der Organisation freigeben können. Sie müssen diese externen Benutzerlizenzen nicht erteilen. Sie müssen auch keine Konten für Sie hinzufügen, es sei denn, die Freigabe ist auf "nur vorhandene externe Benutzer" festgelegt. Wenn die Personen in diesem Fall nicht im Verzeichnis Ihrer Organisation sind, müssen Sie diese als Gastbenutzer im Azure AD Admin Center hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1d870-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

