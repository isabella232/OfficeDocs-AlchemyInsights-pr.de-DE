---
title: Problembehandlung bei Zugriff verweigerten Nachrichten
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503527"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="e8b9f-102">Problembehandlung bei Zugriff verweigerten Nachrichten in SharePoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="e8b9f-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="e8b9f-103">Wenn Sie eine Meldung zum Zugriff verweigert erhalten, wenn Sie versuchen, zu einem SharePoint/OneDrive Admin Center zu navigieren, stellen Sie sicher, dass Sie [dem Benutzer eine Lizenz zuweisen](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="e8b9f-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="e8b9f-104">Wenn der Benutzer über eine Lizenz verfügt, sollten Sie auch sicherstellen, dass ihm [eine Administratorrolle zugewiesen](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) ist, die auf die Admin Center zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="e8b9f-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="e8b9f-105">Dieses Problem kann auch auftreten, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e8b9f-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e8b9f-106">Das neue Konto wird mithilfe eines anderen Werts für PUID (Passport Unique ID) erstellt.</span><span class="sxs-lookup"><span data-stu-id="e8b9f-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e8b9f-107">Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, verfügt der Benutzer über eine falsche PUID.</span><span class="sxs-lookup"><span data-stu-id="e8b9f-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e8b9f-108">Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory Organisationseinheit (Organizational Unit, OU).</span><span class="sxs-lookup"><span data-stu-id="e8b9f-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e8b9f-109">Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint erneut synchronisiert wurden, kann dieses Problem auftreten.</span><span class="sxs-lookup"><span data-stu-id="e8b9f-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="e8b9f-110">Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel wiederherstellen, [einen Benutzer in Office 365 wiederherstellen](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e8b9f-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="e8b9f-111">Hinweis: Wenn ein OneDrive-oder SharePoint Admin Center nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, ist möglicherweise ein vorübergehendes Dienst Problem aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="e8b9f-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="e8b9f-112">[Überprüfen Sie das Dienst Integritäts Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e8b9f-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


