---
title: Workflow-e-Mail wird nicht gesendet
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270671"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="8cc59-102">Workflow-e-Mail wird nicht gesendet</span><span class="sxs-lookup"><span data-stu-id="8cc59-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="8cc59-103">E-Mails aus Workflows werden nicht an alle Benutzer oder nur bestimmte Benutzer gesendet, oder es wird der Fehler angezeigt, dass **die e-Mail-Nachricht nicht gesendet werden kann. Stellen Sie sicher, dass die e-Mail über einen gültigen Empfänger verfügt**.</span><span class="sxs-lookup"><span data-stu-id="8cc59-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="8cc59-104">Überprüfen Sie, ob der Benutzer in der Gruppe **alle Personen** Berechtigungen (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="8cc59-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="8cc59-105">Beispiel für eine direkte URL<tenant>: https://<sitename>. SharePoint.com/Sites//_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="8cc59-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="8cc59-106">Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist.</span><span class="sxs-lookup"><span data-stu-id="8cc59-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="8cc59-107">Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass Ihre Einladung akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="8cc59-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="8cc59-108">Wenn der Benutzer in der Gruppe Berechtigungen vorhanden ist, stellen Sie sicher, dass die e-Mail-Adresse richtig ist.</span><span class="sxs-lookup"><span data-stu-id="8cc59-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="8cc59-109">Wenn die e-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielwarnung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos von Benutzerprofilen von SharePoint zu dieser Websitesammlung erzwingt.</span><span class="sxs-lookup"><span data-stu-id="8cc59-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="8cc59-110">E-Mails aus Workflows werden an die Websitesammlungsadministratoren, jedoch nicht an andere Benutzer gesendet, und es wird der Fehler " \*\*http verboten <spam> <spam> \*\* <spam> <spam>" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8cc59-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="8cc59-111">Siehe [Zugriff verweigert, wenn e-Mails an Gruppen gesendet werden](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="8cc59-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="8cc59-112">Stellen Sie außerdem sicher, dass das Feature für die **Sperrung der Benutzerberechtigungen für den begrenzten Zugriff** nicht aktiv ist.</span><span class="sxs-lookup"><span data-stu-id="8cc59-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="8cc59-113">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="8cc59-113">Related topics</span></span>
<span data-ttu-id="8cc59-114">Möchten Sie Microsoft Flow in SharePoint Online testen?</span><span class="sxs-lookup"><span data-stu-id="8cc59-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="8cc59-115">Fluss erstellen</span><span class="sxs-lookup"><span data-stu-id="8cc59-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8cc59-116">SharePoint und Flow</span><span class="sxs-lookup"><span data-stu-id="8cc59-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


