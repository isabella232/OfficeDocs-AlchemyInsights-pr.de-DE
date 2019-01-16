---
title: Gewähren des Benutzerzugriffs auf SharePoint und OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 5a1cdeefa4474e8ce0e6a7a37be016cc87b9791d
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289494"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="998cb-102">Gewähren des Benutzerzugriffs auf SharePoint und OneDrive</span><span class="sxs-lookup"><span data-stu-id="998cb-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="998cb-p101">Eine OneDrive oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die bisher zugreifen, möglicherweise ein temporäres Problem. [Überprüfen Sie die Dienst-Statusanzeige](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="998cb-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="998cb-p102">Wenn Sie Personen in Ihrer Organisation möglich an-und SharePoint- und OneDrive verwenden möchten, müssen Sie für diese Konten hinzufügen, und stellen Sie sicher, dass sie über eine Lizenz verfügen, die Zugriff auf SharePoint und OneDrive gewährt wird. Die einfachste Möglichkeit zum Hinzufügen von Benutzern ist im Office 365 Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="998cb-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="998cb-107">Wechseln Sie auf der [Seite der aktiven Benutzer im Office 365 Administrationscenter](https://portal.office.com/adminportal/home#/users), und klicken Sie dann auf **Benutzer hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="998cb-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="998cb-108">Füllen Sie die Informationen für den Benutzer, und stellen Sie sicher, dass unter **Lizenzen**, eine Lizenz zugewiesen ist, und **SharePoint Online** ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="998cb-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="998cb-p103">Beachten Sie, dass Benutzer, wenn Sie externe Freigabe in Ihrer Organisation zulassen, SharePoint und OneDrive Inhalte mit Personen außerhalb der Organisation freigeben können. Sie müssen nicht diese Lizenzen für externe Benutzer angeben. Nicht müssen Sie auch für diese Konten hinzufügen, wenn die Freigabe auf "Nur vorhandene externe Benutzer." festgelegt ist In diesem Fall müssen Sie die Personen in Ihrer Organisation Verzeichnis nicht, sie als Gastbenutzer in der Azure AD-Verwaltungskonsole hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="998cb-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

