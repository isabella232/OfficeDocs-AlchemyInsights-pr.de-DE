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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059603"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="51cab-102">Workflow-e-Mail wird nicht gesendet</span><span class="sxs-lookup"><span data-stu-id="51cab-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="51cab-103">E-Mails aus Workflows werden nicht an alle Benutzer oder nur bestimmte Benutzer gesendet, oder es wird der Fehler angezeigt, dass **die e-Mail-Nachricht nicht gesendet werden kann. Stellen Sie sicher, dass die e-Mail über einen gültigen Empfänger verfügt**.</span><span class="sxs-lookup"><span data-stu-id="51cab-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="51cab-104">Überprüfen Sie, ob der Benutzer in der Gruppe **alle Personen** Berechtigungen (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="51cab-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="51cab-105">Beispiel für eine direkte URL<tenant>: https://<sitename>. SharePoint.com/Sites//_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="51cab-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="51cab-106">Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist.</span><span class="sxs-lookup"><span data-stu-id="51cab-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="51cab-107">Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass Ihre Einladung akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="51cab-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="51cab-108">Wenn der Benutzer in der Gruppe Berechtigungen vorhanden ist, stellen Sie sicher, dass die e-Mail-Adresse richtig ist.</span><span class="sxs-lookup"><span data-stu-id="51cab-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="51cab-109">Wenn die e-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielwarnung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos von Benutzerprofilen von SharePoint zu dieser Websitesammlung erzwingt.</span><span class="sxs-lookup"><span data-stu-id="51cab-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="51cab-110">E-Mails aus Workflows werden an die Websitesammlungsadministratoren, jedoch nicht an andere Benutzer gesendet, und es wird der Fehler " \*\*http verboten <spam> <spam> \*\* <spam> <spam>" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="51cab-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="51cab-111">Siehe [Zugriff verweigert, wenn e-Mails an Gruppen gesendet werden](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="51cab-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="51cab-112">Stellen Sie außerdem sicher, dass das Feature für die **Sperrung der Benutzerberechtigungen für den begrenzten Zugriff** nicht aktiv ist.</span><span class="sxs-lookup"><span data-stu-id="51cab-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="51cab-113">Verwandte Themen</span><span class="sxs-lookup"><span data-stu-id="51cab-113">Related topics</span></span>
- [<span data-ttu-id="51cab-114">Fluss erstellen</span><span class="sxs-lookup"><span data-stu-id="51cab-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="51cab-115">SharePoint und Flow</span><span class="sxs-lookup"><span data-stu-id="51cab-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


