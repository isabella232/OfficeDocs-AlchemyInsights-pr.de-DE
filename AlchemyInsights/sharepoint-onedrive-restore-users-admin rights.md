---
title: Gewähren von Benutzern Zugriff auf SharePoint und OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736647"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="4419c-102">Gewähren von Benutzern Zugriff auf SharePoint und OneDrive</span><span class="sxs-lookup"><span data-stu-id="4419c-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="4419c-103">Dieses Problem tritt am häufigsten auf, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="4419c-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4419c-104">Das neue Konto wird mithilfe eines anderen Werts für PUID (Passport Unique ID) erstellt.</span><span class="sxs-lookup"><span data-stu-id="4419c-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4419c-105">Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, verfügt der Benutzer über eine falsche PUID.</span><span class="sxs-lookup"><span data-stu-id="4419c-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4419c-106">Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory Organisationseinheit (Organizational Unit, OU).</span><span class="sxs-lookup"><span data-stu-id="4419c-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4419c-107">Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint erneut synchronisiert wurden, kann dieses Problem auftreten.</span><span class="sxs-lookup"><span data-stu-id="4419c-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4419c-108">Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel wiederherstellen, indem Sie[einen Benutzer in Office 365 wiederherstellen](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4419c-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="4419c-109">Nachdem Sie dies abgeschlossen haben, können Sie überprüfen, ob der Benutzer Administratorrechte für die OneDrive-Website hat, indem Sie die Schritte zum [Hinzufügen von Administratoren für die OneDrive eines Benutzers](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) ausführen.</span><span class="sxs-lookup"><span data-stu-id="4419c-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="4419c-110">Weitere Informationen zu Berechtigungsstufen finden Sie im Artikel [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4419c-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
