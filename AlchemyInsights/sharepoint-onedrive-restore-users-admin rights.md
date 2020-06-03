---
title: Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive für Unternehmen Websites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511183"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="06a91-102">Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive für Unternehmen Websites</span><span class="sxs-lookup"><span data-stu-id="06a91-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="06a91-103">Dieses Problem tritt am häufigsten auf, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="06a91-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="06a91-104">Das neue Konto wird mithilfe eines anderen Werts für PUID (Passport Unique ID) erstellt.</span><span class="sxs-lookup"><span data-stu-id="06a91-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="06a91-105">Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, verfügt der Benutzer über eine falsche PUID.</span><span class="sxs-lookup"><span data-stu-id="06a91-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="06a91-106">Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory Organisationseinheit (Organizational Unit, OU).</span><span class="sxs-lookup"><span data-stu-id="06a91-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="06a91-107">Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint erneut synchronisiert wurden, kann dieses Problem auftreten.</span><span class="sxs-lookup"><span data-stu-id="06a91-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="06a91-108">Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten in diesem Artikel wiederherstellen, um [einen Benutzer in Microsoft 365 wiederherzustellen](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="06a91-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="06a91-109">Wenn Sie den ursprünglichen Benutzer nicht wiederherstellen können, sollten Sie den alten Benutzer aus der OneDrive-Website mithilfe dieser Schritte entfernen, indem Sie [einen Benutzer aus der Liste Benutzerinformationen entfernen]().</span><span class="sxs-lookup"><span data-stu-id="06a91-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="06a91-110">Nachdem Sie dies abgeschlossen haben, können Sie überprüfen, ob der Benutzer Administratorrechte für die OneDrive-Website hat, indem Sie die Schritte zum [Hinzufügen von Administratoren für die OneDrive eines Benutzers](https://docs.microsoft.com/sharepoint/manage-user-profiles) ausführen.</span><span class="sxs-lookup"><span data-stu-id="06a91-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="06a91-111">Weitere Informationen zu Berechtigungsstufen finden Sie im Artikel [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="06a91-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
