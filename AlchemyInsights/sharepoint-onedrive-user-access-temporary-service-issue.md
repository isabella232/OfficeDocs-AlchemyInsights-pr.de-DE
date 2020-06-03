---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511147"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="d1230-102">SharePoint oder OneDrive langsam, unzugänglich oder nicht verfügbar für mehrere Benutzer</span><span class="sxs-lookup"><span data-stu-id="d1230-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="d1230-103">Wenn eine OneDrive-oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, ist möglicherweise ein vorübergehendes Dienst Problem aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="d1230-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="d1230-104">[Überprüfen Sie das Dienst Integritäts Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d1230-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="d1230-105">**Hinzufügen und lizenzieren des Benutzers**</span><span class="sxs-lookup"><span data-stu-id="d1230-105">**Add and license the user**</span></span>

<span data-ttu-id="d1230-106">Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 for Business Lizenzen zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="d1230-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="d1230-107">**Zuweisen von Berechtigungen**</span><span class="sxs-lookup"><span data-stu-id="d1230-107">**Assign Permissions**</span></span>

<span data-ttu-id="d1230-108">Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und weiterhin eine Nachricht mit Zugriff verweigert erhalten wird, stellen Sie sicher, dass Ihnen die [entsprechende Berechtigungsstufe](https://docs.microsoft.com/sharepoint/understanding-permission-levels) zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="d1230-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="d1230-109">**Verwenden der Access-Anforderungsfunktion in Frage stellen**</span><span class="sxs-lookup"><span data-stu-id="d1230-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="d1230-110">Mit der [Zugriffs Anforderungsfunktion](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) können Benutzer Zugriff auf Inhalte anfordern, für die Sie derzeit keine Berechtigung haben.</span><span class="sxs-lookup"><span data-stu-id="d1230-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="d1230-111">**Benutzerdefiniertes Skript zulassen verursacht möglicherweise Zugriffs Verweigerungs Probleme**</span><span class="sxs-lookup"><span data-stu-id="d1230-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="d1230-112">Es gibt bestimmte Szenarien, in denen das Feature *benutzerdefiniertes Skript zulassen* möglicherweise einen Zugriff verweigert darstellt.</span><span class="sxs-lookup"><span data-stu-id="d1230-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="d1230-113">Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="d1230-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="d1230-114">Weitere Informationen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="d1230-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

