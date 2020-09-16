---
title: Workflow-e-Mail wird nicht gesendet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748988"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="adf01-102">Workflow-e-Mails werden nicht für eine SharePoint-Liste oder-Bibliothek gesendet.</span><span class="sxs-lookup"><span data-stu-id="adf01-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="adf01-103">E-Mails aus Workflows werden nicht an alle Benutzer oder nur bestimmte Benutzer gesendet, oder es wird der Fehler angezeigt, dass **die e-Mail-Nachricht nicht gesendet werden kann. Stellen Sie sicher, dass die e-Mail über einen gültigen Empfänger verfügt**.</span><span class="sxs-lookup"><span data-stu-id="adf01-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="adf01-104">Überprüfen Sie, ob der Benutzer in der Gruppe **alle Personen** Berechtigungen (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="adf01-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="adf01-105">Beispiel für eine direkte URL: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="adf01-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="adf01-106">Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist.</span><span class="sxs-lookup"><span data-stu-id="adf01-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="adf01-107">Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass Ihre Einladung akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="adf01-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="adf01-108">Wenn der Benutzer in der Gruppe Berechtigungen vorhanden ist, stellen Sie sicher, dass die e-Mail-Adresse richtig ist.</span><span class="sxs-lookup"><span data-stu-id="adf01-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="adf01-109">Wenn die e-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielwarnung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos von Benutzerprofilen von SharePoint zu dieser Websitesammlung erzwingt.</span><span class="sxs-lookup"><span data-stu-id="adf01-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="adf01-110">E-Mails aus Workflows werden an die Websitesammlungsadministratoren, jedoch nicht an andere Benutzer gesendet, und es wird der Fehler " **http verboten" für <span>https angezeigt:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="adf01-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="adf01-111">Siehe [Zugriff verweigert, wenn Sie eine e-Mail an eine SharePoint-Gruppe senden](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="adf01-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="adf01-112">Stellen Sie außerdem sicher, dass das Feature für die **Sperrung der Benutzerberechtigungen für den begrenzten Zugriff** nicht aktiv ist.</span><span class="sxs-lookup"><span data-stu-id="adf01-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="adf01-113">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="adf01-113">Related topics</span></span>
<span data-ttu-id="adf01-114">Möchten Sie Microsoft Flow in SharePoint Online testen?</span><span class="sxs-lookup"><span data-stu-id="adf01-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="adf01-115">Fluss erstellen</span><span class="sxs-lookup"><span data-stu-id="adf01-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="adf01-116">SharePoint und Flow</span><span class="sxs-lookup"><span data-stu-id="adf01-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


