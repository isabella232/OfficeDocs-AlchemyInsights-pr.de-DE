---
title: Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive für Unternehmen Websites
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
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223423"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive für Unternehmen Websites

Dieses Problem tritt am häufigsten auf, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen Werts für PUID (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, verfügt der Benutzer über eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory Organisationseinheit (Organizational Unit, OU). Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint erneut synchronisiert wurden, kann dieses Problem auftreten.

Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel wiederherstellen, indem Sie[einen Benutzer in Office 365 wiederherstellen](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Nachdem Sie dies abgeschlossen haben, können Sie überprüfen, ob der Benutzer Administratorrechte für die OneDrive-Website hat, indem Sie die Schritte zum [Hinzufügen von Administratoren für die OneDrive eines Benutzers](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) ausführen.

Weitere Informationen zu Berechtigungsstufen finden Sie im Artikel [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
