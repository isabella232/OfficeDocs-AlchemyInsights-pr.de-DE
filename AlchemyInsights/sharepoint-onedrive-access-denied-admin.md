---
title: Behandeln von Zugriffs verweigerten Nachrichten
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707953"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="4e5f6-102">Behandeln von Zugriffs verweigerten Nachrichten in Sharepoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="4e5f6-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="4e5f6-103">Wenn Sie beim Versuch, zu einem Sharepoint/OneDrive Admin Center zu navigieren, eine Nachricht mit dem Zugriff verweigert erhalten, stellen Sie sicher, dass Sie dem Benutzer eine [Lizenz zuweisen.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="4e5f6-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="4e5f6-104">Wenn der Benutzer über eine Lizenz verfügt, sollten Sie auch sicherstellen, dass ihm eine Administratorrolle zugewiesen ist, [die](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) auf die Admin Center zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="4e5f6-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="4e5f6-105">Dieses Problem kann auch auftreten, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="4e5f6-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4e5f6-106">Das neue Konto wird mithilfe eines anderen PUID -Werts (Passport Unique ID) erstellt.</span><span class="sxs-lookup"><span data-stu-id="4e5f6-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4e5f6-107">Wenn der Benutzer versucht, auf eine Websitesammlung oder sein OneDrive zu zugreifen, hat der Benutzer eine falsche PUID.</span><span class="sxs-lookup"><span data-stu-id="4e5f6-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4e5f6-108">Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory-Organisationseinheit (Ou).</span><span class="sxs-lookup"><span data-stu-id="4e5f6-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4e5f6-109">Wenn benutzer sich bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint neu synchronisiert werden, kann dieses Problem auf sie bzw. die Benutzer bzw. die Benutzerin sharePoint angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="4e5f6-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4e5f6-110">Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel Wiederherstellen eines Benutzers [in Microsoft 365 wiederherstellen.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="4e5f6-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="4e5f6-111">Hinweis: Wenn ein OneDrive- oder SharePoint Admin Center nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein temporäres Dienstproblem vorliegen.</span><span class="sxs-lookup"><span data-stu-id="4e5f6-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="4e5f6-112">[Überprüfen Sie das Dienstintegashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4e5f6-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


